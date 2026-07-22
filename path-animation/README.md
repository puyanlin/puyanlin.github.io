# 路徑動畫 Path Animation

單一靜態 HTML（`index.html`），SVG + 原生 JS 路徑動畫，無任何依賴、無 build step。

## 動畫順序
1. ①（右上黃綠）沿 P1 斜穿中央到左下箭頭
2. ②（左邊橘黑）沿 P2 斜穿中央到右下箭頭
3. ③（右下紅白）沿 P3 繞右側越過頂端到左上箭頭
4. ① 滑到 P2 起點，沿 ② 剛走過的路徑走回右邊

## 調整路徑
三條路徑的 SVG `d` 值在 `index.html` 的 `<path id="p1|p2|p3">`，座標系 1176x680，直接改即可。
動畫時序在 `<script>` 內的 `legs` 陣列（順序、秒數、標籤）。

## 部署
GitHub Pages：Settings → Pages → Deploy from a branch → main / root。
或 Vercel：直接 import 此 repo，零設定。
