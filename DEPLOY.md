# 部署指南

## 🚀 快速部署到 Vercel（推薦）

### 方法一：通過 Vercel 網頁界面（最簡單）

1. **前往 Vercel**
   - 打開 https://vercel.com
   - 使用 GitHub 帳號登入

2. **導入專案**
   - 點擊 "Add New Project" 或 "Import Project"
   - 選擇 GitHub repository: `enya0911/self-growth-leadership`
   - 點擊 "Import"

3. **配置專案**
   - Project Name: `self-growth-leadership`（或自訂名稱）
   - Framework Preset: Other（或留空，因為是靜態 HTML）
   - Root Directory: `./`（預設）
   - Build Command: 留空（靜態網站不需要 build）
   - Output Directory: `./`（預設）

4. **部署**
   - 點擊 "Deploy"
   - 等待 1-2 分鐘完成部署
   - 部署完成後會獲得 URL，例如：`https://self-growth-leadership.vercel.app`

5. **設定自訂網域（選用）**
   - 在專案設定中可以添加自訂網域
   - 例如：`self-growth-leadership.yourdomain.com`

### 方法二：使用 Vercel CLI

```bash
# 1. 安裝 Vercel CLI
npm install -g vercel

# 2. 登入 Vercel
vercel login

# 3. 在專案目錄執行部署
cd /Users/samuelhou/self-growth-leadership
vercel

# 4. 生產環境部署
vercel --prod
```

### 方法三：使用 GitHub Pages

1. **啟用 GitHub Pages**
   - 前往 https://github.com/enya0911/self-growth-leadership/settings/pages
   - Source: Deploy from a branch
   - Branch: `main`
   - Folder: `/ (root)`
   - 點擊 "Save"

2. **等待部署**
   - 幾分鐘後，網站會在以下網址上線：
   - `https://enya0911.github.io/self-growth-leadership`

## 📝 部署後的步驟

1. **記下部署 URL**
   - Vercel: `https://self-growth-leadership-xxx.vercel.app`
   - GitHub Pages: `https://enya0911.github.io/self-growth-leadership`

2. **更新整合代碼**
   - 打開 `personal-website-integration.html`
   - 將所有 `https://self-growth-leadership.vercel.app` 替換為實際的部署 URL

3. **測試連結**
   - 確認所有連結正常運作
   - 測試返回個人網站的連結
   - 測試報名表單功能

## 🔗 整合到個人網站

部署完成後，按照 `INTEGRATION.md` 中的說明，將代碼添加到個人網站的「成長領導」區塊。

## ✅ 檢查清單

- [ ] 代碼已推送到 GitHub
- [ ] 在 Vercel 或 GitHub Pages 部署完成
- [ ] 獲得部署 URL
- [ ] 測試網站功能正常
- [ ] 更新整合代碼中的 URL
- [ ] 在個人網站中添加服務連結
- [ ] 測試從個人網站到服務網站的連結
- [ ] 測試返回個人網站的連結

