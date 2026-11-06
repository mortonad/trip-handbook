# 把「九州行動手冊」上架成公開網站（GitHub Pages）

上架後會得到一個**公開網址**，你和旅伴**各自手機點開就能用、不用登入**；手機上按「加到主畫面」就變成 App、還能**離線**（靠 sw.js 快取）。全程**免費**。

這個資料夾要上傳的 5 個檔：`index.html`、`manifest.json`、`sw.js`、`icon-192.png`、`icon-512.png`。

---

## 三步驟（手機或電腦都能做，用 GitHub 網頁版）

### 1. 開一個 GitHub repository
- 到 **github.com** 登入（沒有帳號就免費註冊）。
- 右上「＋」→ **New repository**。
- Repository name 隨意，例如 **`kyushu-trip`**；選 **Public**；按 **Create repository**。

### 2. 上傳這 5 個檔
- 在新 repo 頁面點 **Add file → Upload files**。
- 把這個資料夾裡的 **index.html、manifest.json、sw.js、icon-192.png、icon-512.png** 全部拖進去（**不要連同資料夾，直接放這 5 個檔在最上層**）。
- 下面按 **Commit changes**。

### 3. 開啟 Pages
- repo 上方 **Settings → 左欄 Pages**。
- **Source** 選「**Deploy from a branch**」。
- **Branch** 選 **main**、資料夾選 **/ (root)** → **Save**。
- 等 1–2 分鐘重新整理，同一頁最上面會出現網址：
  **`https://<你的帳號>.github.io/kyushu-trip/`**
- 把這個網址給旅伴即可。

---

## 用法與提醒
- **加到主畫面變 App**：手機瀏覽器開網址 → 分享／選單 → 「加到主畫面」。之後離線也能開（第一次要先連網載入一次）。
- **要更新內容**：改好檔案後，到 repo 重新 Upload files 覆蓋，並把 `sw.js` 裡的 `kyushu-v1` 改成 `kyushu-v2`（讓手機抓新版）。
- **隱私**：Public repo 代表網址知道的人都看得到。裡面只有行程、店家、公開電話，**沒有**預約番號或個資，放公開沒問題。
- 想改成不公開又能分享，可改用 Cloudflare Pages / Netlify，但步驟較多；一般 Public 就夠用。

需要我幫你改內容或換版本，再把檔案丟回來即可。
