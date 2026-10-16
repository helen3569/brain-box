# 腦袋收納盒

隨手記下想做的事，自動分到「想買」「行程」「想做」「記事板」，做完打勾。

網址：https://helen3569.github.io/brain-box/

## 同步（不用登入）

資料存在 Firebase Firestore，用「同步碼」區分：每台裝置用同一組同步碼，資料就會同步。

- 第一台裝置打開網站會自動產生同步碼。
- 「記下」頁最下面「同步與備份」→「複製同步連結」，傳到其他裝置打開一次就會連上。
- 同步連結不要給別人，拿到的人也看得到資料。

Firestore 的「規則」要貼上 `firestore.rules` 的內容並發布。

## 更新版面

把新的 `index.html`（或其他改過的檔案）拖到 GitHub repo 的 Add file → Upload files，Commit 後 1～2 分鐘生效。
