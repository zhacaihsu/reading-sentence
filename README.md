# 認字拼字 PWA：中文拼句 + 英文拼字

將 ZIP 解壓縮，並把 `index.html`、`sw.js`、`manifest.webmanifest`、`icons/` 資料夾及 `.nojekyll` 上傳至 GitHub Repository 根目錄。GitHub → Settings → Pages → Deploy from a branch → main → /(root)。提交並等待 Pages 部署成功。

## 英文練習

- 預設範例：cat、dog、sun、hat、pen、cup、bus、bed、pig、fish、book、apple。
- 題目在上方，下面有逐字母的格子。點字母念出英文字母名稱，按照點選順序填格；可取消、清空、重排。整個單字按「朗讀拼好的單字」。
- 預設只顯示單字需要的打亂字母；可切換完整 A–Z 26 個字母，支援重複字母（book、apple）。
- 英文單字須為 2–15 個英文字母，可新增、編輯、刪除、選題、匯出/匯入 JSON。
- 中文題庫保留第三版資料鍵值及 JSON 相容性；英文使用獨立題庫，不會覆蓋中文。
- 語速可調 0.5–1.5 倍。英文語音由瀏覽器/裝置的英語語音引擎負責，單字朗讀效果取決於語音引擎；字母名稱與拼讀自然音不同。

## 隱私與備份

自訂題目保存在瀏覽器 localStorage。不同手機不會自動同步；需使用 JSON 匯出、匯入。請避免用無痕模式保存重要題庫。離線瀏覽依 PWA service worker 快取，離線語音是否可用取決於手機是否有離線語音包。
