# 認字拼句練習 — PWA 模式一

## 使用方式
上方顯示題目與逐字空格。點選下方打亂順序的字卡時，會朗讀單字並依照點選順序填入下一個空格。支援取消上一字、清除全部、朗讀目前拼好的句子、聽題目及修改題目。

## 上傳到 GitHub Pages
1. 建立 Public repository（例如 `reading-sentence`）。
2. 將本資料夾內的 `index.html`、`manifest.webmanifest`、`sw.js`、`icons` 資料夾及 `.nojekyll` 上傳到 repository 根目錄，並按 **Commit changes**。
3. 前往 **Settings → Pages → Build and deployment**。
4. Source 選 **Deploy from a branch**，Branch 選 **main**，資料夾選 **/(root)**，按 **Save**。
5. 網站網址格式為 `https://你的帳號.github.io/reading-sentence/`。
6. 以 Android Chrome 開啟網址，從右上角選單選「安裝應用程式」或「加到主畫面」。iPad 使用 Safari 分享選單「加入主畫面」。

## 注意
- GitHub Pages 必須透過 HTTPS 開啟才能啟用 PWA 離線快取；直接開本機 HTML 不能測試安裝與離線。
- 首次使用需連網，載入完成後頁面可以離線開啟。語音使用瀏覽器/系統語音合成服務，部分裝置即使頁面離線也可能無法朗讀；請先在目標裝置測試。
- 設定的句子目前不會永久儲存，重新開啟會回到預設題目。
- 若更新 app 檔案，請將 `sw.js` 內 CACHE_NAME 版本加一以更新離線快取。
