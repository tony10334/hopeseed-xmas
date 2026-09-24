# 小花

交換禮物互動懸疑遊戲《小花》的共用頁面。以 GitHub Pages 提供靜態頁面，遊戲進度存放在 Firebase Firestore，主持人更新後所有玩家即時同步。

## 檔案

- `index.html`：整個頁面（由另一個工作資料夾的 `build.py` 產生，請勿手改）。
- `config.js`：Firebase 專案設定，貼上 Firebase 主控台給的 `firebaseConfig`。
- `firestore.rules`：Firestore 安全規則，貼到 Firebase 主控台的 Firestore → 規則。

## Firebase 設定

1. 建立 Firebase 專案，新增「網頁應用程式」，把 `firebaseConfig` 內容填進 `config.js`。
2. Firestore Database：建立資料庫（asia-east1），把 `firestore.rules` 的內容貼到「規則」並發布。
3. Authentication：啟用「匿名」與「Google」兩種登入方式；在「設定 → 授權網域」加入這個網站的網域（例如 `xxx.github.io`）。

## 主持人

打開頁面，最下方「主持人登入」用 Google 帳號登入。第一個登入的帳號會成為主持人。之後其他 Google 帳號登入會送出申請，主持人在「主持手冊」分頁的「共同主持人」區核准或拒絕，也可以移除已加入的主持人。
