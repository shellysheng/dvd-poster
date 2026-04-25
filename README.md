# 📀 新片新書貼文產生器

## 部署步驟

### 第一步：把檔案放到 GitHub

1. 登入 [github.com](https://github.com)
2. 點右上角 **+** → **New repository**
3. Repository name 填 `dvd-poster`
4. 選 **Public**，按 **Create repository**
5. 點 **uploading an existing file**，把以下三個檔案全部拖進去：
   - `index.html`
   - `netlify.toml`
   - `netlify/functions/analyze.js`
6. 按 **Commit changes**

### 第二步：連接 Netlify

1. 登入 [netlify.com](https://netlify.com)（可用 GitHub 帳號登入）
2. 點 **Add new site** → **Import an existing project**
3. 選 **GitHub**，選剛才建立的 `dvd-poster` repository
4. 直接按 **Deploy** 就好

### 第三步：設定 API 金鑰

1. 到 [console.anthropic.com/settings/keys](https://console.anthropic.com/settings/keys) 取得 API 金鑰
2. 回到 Netlify，進入你的 site → **Site configuration** → **Environment variables**
3. 點 **Add a variable**：
   - Key：`ANTHROPIC_API_KEY`
   - Value：貼上你的 API 金鑰（sk-ant-...）
4. 按 **Save**，然後到 **Deploys** 頁面按 **Trigger deploy**

### 完成！

Netlify 會給你一個網址（例如 `https://dvd-poster-abc123.netlify.app`），
把這個網址透過 LINE 傳給媽媽，存到手機書籤就可以隨時使用！
