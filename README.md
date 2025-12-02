# 自我成長領導力網站

## 部署指南

### 方法一：GitHub Pages（推薦）

1. **在 GitHub 建立新 repository**
   - 前往 https://github.com/new
   - 輸入 repository 名稱（例如：`self-growth-leadership`）
   - 選擇 Public（公開）
   - 點擊 "Create repository"

2. **將專案推送到 GitHub**
   ```bash
   # 初始化 git（如果還沒有）
   git init
   
   # 添加所有文件
   git add .
   
   # 提交
   git commit -m "Initial commit"
   
   # 添加遠端 repository（替換 YOUR_USERNAME 和 REPO_NAME）
   git remote add origin https://github.com/YOUR_USERNAME/REPO_NAME.git
   
   # 推送到 GitHub
   git branch -M main
   git push -u origin main
   ```

3. **啟用 GitHub Pages**
   - 前往 repository 的 Settings
   - 左側選單點擊 "Pages"
   - Source 選擇 "Deploy from a branch"
   - Branch 選擇 "main"，資料夾選擇 "/ (root)"
   - 點擊 "Save"
   - 幾分鐘後，網站會在 `https://YOUR_USERNAME.github.io/REPO_NAME` 上線

### 方法二：Netlify（最簡單，支援拖放）

1. **前往 Netlify**
   - 前往 https://www.netlify.com/
   - 註冊/登入帳號（可用 GitHub 帳號登入）

2. **部署網站**
   - 點擊 "Add new site" → "Deploy manually"
   - 直接將整個專案資料夾拖放到頁面上
   - 或使用 Netlify CLI：
     ```bash
     # 安裝 Netlify CLI
     npm install -g netlify-cli
     
     # 登入
     netlify login
     
     # 部署
     netlify deploy --prod
     ```

3. **設定自訂網域（選用）**
   - 在 Netlify 控制台可以設定自訂網域

### 方法三：Vercel

1. **安裝 Vercel CLI**
   ```bash
   npm install -g vercel
   ```

2. **部署**
   ```bash
   # 在專案目錄執行
   vercel
   
   # 生產環境部署
   vercel --prod
   ```

### 方法四：Cloudflare Pages

1. **前往 Cloudflare Pages**
   - 前往 https://pages.cloudflare.com/
   - 登入 Cloudflare 帳號

2. **連接 GitHub repository**
   - 點擊 "Create a project"
   - 選擇 GitHub repository
   - 設定：
     - Build command: （留空，因為是靜態網站）
     - Build output directory: `/`
   - 點擊 "Save and Deploy"

## 本地測試

在部署前，可以先在本地測試：

```bash
# 使用 Python（如果已安裝）
python3 -m http.server 8000

# 或使用 Node.js
npx serve

# 然後在瀏覽器打開
# http://localhost:8000
```

## 注意事項

- 確保所有圖片路徑都是相對路徑（已確認使用 `images/`）
- 確保 `index.html` 在根目錄
- 如果使用自訂網域，記得設定 DNS 記錄

