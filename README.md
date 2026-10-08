# TOEIC 900 Vocabulary — PWA STRICT v5

這是可安裝的 PWA 版本，專為 TOEIC 825 → 900 設計。

## 重要
直接從 Android 檔案管理員開 `index.html` 只能預覽，**不能觸發 PWA 安裝**。
PWA 安裝需要以 HTTPS 網址開啟（localhost 例外）。

## 檔案
- index.html
- style.css
- app.js
- manifest.webmanifest
- service-worker.js
- icons/icon-192.png
- icons/icon-512.png

## 最簡單部署方式

### GitHub Pages
1. 新建一個 GitHub repository。
2. 把本資料夾內所有檔案上傳到 repository 根目錄。
3. Repository → Settings → Pages。
4. Build and deployment 選 `Deploy from a branch`。
5. Branch 選 `main` / `(root)`。
6. 等 GitHub Pages 產生 HTTPS 網址。
7. 用 Android Chrome 開該網址。
8. 右上角 `⇩` 或 Chrome 選單中的「安裝應用程式」即可安裝。

### Netlify
把整個資料夾拖到 Netlify Drop，即可取得 HTTPS 網址。

## Android 安裝條件
- 使用 HTTPS 網址。
- Chrome / Edge 等支援 PWA 的瀏覽器。
- manifest 與 service worker 可正常讀取。
- 瀏覽器判定符合安裝條件後，右上角會出現 `⇩` 安裝按鈕。

## iPhone / iPad
Safari → 分享 → 加入主畫面。

## 離線
Service Worker 會快取 App 外殼；字庫資料仍由 App 的 IndexedDB 保存。


## Responsive desktop layout
- Mobile: bottom navigation, touch-first single-column UI.
- Desktop (>=900px): fixed left sidebar, wide workspace, 4–5 column deck library, centered flashcards/quizzes, 4-column matching game.
- One URL automatically adapts to phone, tablet, and desktop.


## v5.1
Icons are stored in the repository root for simpler GitHub web upload.
