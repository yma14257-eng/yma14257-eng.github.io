# 土建品管刷題場

公共工程品質管理訓練班（土建）115 年 1 月起適用測驗題庫練習，共 2,593 題 / 17 章。

純靜態單檔網頁，沒有後端、沒有外部相依（字型走 Google Fonts CDN，離線時自動退回系統字型）。
作答紀錄、錯題本、未完成的一輪都存在瀏覽器 localStorage，不會上傳到任何地方。

## 部署到 GitHub Pages

1. 建一個新 repo（Public）
2. 上傳 `index.html` 到根目錄
3. Settings → Pages → Source 選 `Deploy from a branch`，Branch 選 `main` / `(root)`，Save
4. 等 1–2 分鐘，網址是 `https://<你的帳號>.github.io/<repo 名稱>/`

## 更新題庫

`index.html` 最底下的 `<script type="application/json" id="qdata">` 就是題庫，
格式為 `{"chapters":[章節名稱...],"q":[[章節索引, 題幹, [四個選項], 正解索引(0=A)], ...]}`。
