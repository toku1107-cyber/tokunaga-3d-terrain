# (有)徳永測量 社屋 3D地形ビューア

UAV写真測量データ（LAZ点群 + オルソ GeoTIFF）から生成された3D地形ビューアです。

## データ仕様

- 座標系: JGD2011 平面直角座標第II系 (EPSG:6670)
- 実寸: 92.8m × 90.1m
- グリッド: 1050 × 1020 セル（有効 850,732 セル）
- 点群: 6,231,929点
- オルソ: GeoTIFFクロップ (4999x4857, rot=0, Q85)

## アクセス

https://toku1107-cyber.github.io/tokunaga-3d-terrain/

## 開発方法

Claude Code (Anthropic社のAIプログラミングアシスタント) が Python スクリプト `generate_3d_viewer.py` を自動生成・更新し、Metashape成果データ（.laz点群・GeoTIFFオルソ）を読み込んで単一HTMLファイル（Three.js 3Dビューア）に変換する方式で開発されています。
