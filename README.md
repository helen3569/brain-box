# 腦袋收納盒

隨手記下想做的事，自動分到「想買」「行程」「想做」「記事板」，做完打勾。

## 設定同步（Firebase，只需做一次）

1. 到 https://console.firebase.google.com 建立專案（Google Analytics 可以關掉）。
2. 左側「Build → Authentication」→ 開始使用 → 「Sign-in method」啟用 **Google**。
3. Authentication →「Settings」→「Authorized domains」→ 新增 `helen3569.github.io`。
4. 左側「Build → Firestore Database」→ 建立資料庫（選 asia-east1 台灣，正式版模式）。
5. Firestore →「規則」，把 `firestore.rules` 的內容整段貼上 → 發布。
6. 專案設定（齒輪）→「一般」→ 下方「你的應用程式」→ 新增 **網頁** 應用程式 → 複製 `firebaseConfig` 裡的值，貼進 `firebase-config.js`。

`firebase-config.js` 裡的 apiKey 是公開識別碼，放在網頁上是正常的；資料安全靠第 5 步的規則保護。

## 搬家

舊版本打開「記下」頁最下面的「備份與搬家」→「複製全部資料」，在新版本同一個地方貼上 →「匯入」。
