# 認字拼句練習 PWA｜第三版（題庫版）

## 功能
- 內建四道不含個資的範例題目。
- 點選題庫句子即可切換出題；點字會朗讀並按點選順序填入空格。
- 自訂題目加入題庫、編輯、刪除、選題。
- 匯出 JSON 備份與匯入 JSON 合併題庫，重複題目自動略過。
- 朗讀速度 0.5～1.5 倍。
- 自訂題庫和語音速度使用 localStorage 保存在使用者自己的瀏覽器，不會上傳至 GitHub，也不會公開給其他使用者。
- 自動嘗試將第二版儲存的自訂句子加入題庫。
- PWA 離線網頁快取。語音離線使用依裝置語音服務而定。

## 部署到 GitHub Pages
1. 將此 ZIP 解壓縮。
2. 上傳解壓縮後的 `index.html`、`sw.js`、`manifest.webmanifest`、`.nojekyll`、`icons/` 到 GitHub Repository **根目錄**，和舊檔同名時選擇覆蓋並 Commit changes。
3. 在 Settings → Pages 選 Deploy from a branch，Branch=`main`、Folder=`/(root)`。
4. Pages 成功部署後，重新開啟 GitHub Pages 網址。如果仍看到舊版，關閉 PWA 再開啟或重新整理。

## 題庫備份格式

```json
{
  "format": "reading-sentence-question-bank",
  "version": 1,
  "exportedAt": "2026-11-19T00:00:00.000Z",
  "sentences": ["我要喝水", "我想看書"]
}
```

匯入只接受以上格式，與 1～20 字的句子。匯入採合併，重複跳過，不清除現有題庫。

## 注意
- GitHub Pages 託管的程式檔案是公開的，但每個使用者自己的題庫只在各自瀏覽器內。任何清除網站資料、使用無痕模式、換裝置的操作，都可能使題庫不見，請定期匯出備份。
- 內建範例不可修改，自己的題目可自行編輯刪除。
