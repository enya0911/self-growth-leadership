# 🚀 立即部署步驟

## 方法：使用 Vercel 網頁界面（推薦，無需安裝任何工具）

### 步驟 1：前往 Vercel（1 分鐘）

1. 打開瀏覽器，前往：**https://vercel.com**
2. 點擊右上角 "Sign Up" 或 "Log In"
3. 選擇 "Continue with GitHub"
4. 授權 Vercel 訪問您的 GitHub 帳號

### 步驟 2：導入專案（2 分鐘）

1. 登入後，點擊 **"Add New Project"** 或 **"Import Project"**
2. 在 "Import Git Repository" 區塊中，找到 **`enya0911/self-growth-leadership`**
3. 如果沒看到，點擊 "Adjust GitHub App Permissions" 確保 Vercel 有權限訪問所有 repositories
4. 選擇 `enya0911/self-growth-leadership` 後，點擊 **"Import"**

### 步驟 3：配置專案（1 分鐘）

在配置頁面：

- **Project Name**: `self-growth-leadership`（或保持預設）
- **Framework Preset**: 選擇 **"Other"** 或留空
- **Root Directory**: `./`（保持預設）
- **Build Command**: **留空**（靜態網站不需要 build）
- **Output Directory**: `./`（保持預設）
- **Install Command**: **留空**

⚠️ **重要**：確保 Build Command 和 Install Command 都是空的！

### 步驟 4：部署（2 分鐘）

1. 點擊 **"Deploy"** 按鈕
2. 等待部署完成（通常 1-2 分鐘）
3. 部署成功後，您會看到：
   - ✅ 綠色的 "Ready" 狀態
   - 🔗 一個 URL，例如：`https://self-growth-leadership-xxx.vercel.app`

### 步驟 5：記下部署 URL

**重要**：請複製並保存這個 URL，稍後需要用它來更新整合代碼！

例如：
```
https://self-growth-leadership-xxx.vercel.app
```

### 步驟 6：測試網站

1. 點擊部署後的 URL，打開網站
2. 確認網站正常顯示
3. 測試導航連結
4. 測試返回個人網站的連結
5. 測試報名表單功能

## ✅ 部署完成後

部署完成後，請執行：

1. **更新整合代碼**
   - 打開 `personal-website-integration.html`
   - 將所有 `https://self-growth-leadership.vercel.app` 替換為您的實際部署 URL

2. **添加到個人網站**
   - 複製更新後的整合代碼
   - 添加到個人網站的「成長領導」區塊

## 🆘 遇到問題？

### 問題 1：找不到 repository
- 確認 GitHub repository 是公開的（Public）
- 確認 Vercel 有權限訪問您的 GitHub

### 問題 2：部署失敗
- 檢查 Build Command 是否為空
- 確認 `vercel.json` 文件存在
- 查看 Vercel 的部署日誌找出錯誤

### 問題 3：網站顯示空白
- 確認 `index.html` 在根目錄
- 檢查圖片路徑是否正確（應該是 `images/xxx.png`）

## 📝 備註

- 部署後，每次推送到 GitHub 的 `main` 分支，Vercel 會自動重新部署
- 可以設定自訂網域（在專案設定中）
- 所有部署都是免費的（Vercel 免費方案）

