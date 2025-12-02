# 🚀 快速開始指南

## 第一步：部署網站

### 推薦方式：Vercel（與個人網站同平台）

1. **前往 Vercel**
   - 打開 https://vercel.com
   - 使用 GitHub 帳號登入（與個人網站相同帳號）

2. **導入專案**
   - 點擊 "Add New Project"
   - 選擇 repository: `enya0911/self-growth-leadership`
   - 點擊 "Import"

3. **配置（使用預設即可）**
   - Project Name: `self-growth-leadership`
   - Framework: Other
   - 其他保持預設

4. **部署**
   - 點擊 "Deploy"
   - 等待 1-2 分鐘
   - **記下部署後的 URL**（例如：`https://self-growth-leadership-xxx.vercel.app`）

## 第二步：更新整合代碼

部署完成後，打開 `personal-website-integration.html`，將所有：
```
https://self-growth-leadership.vercel.app
```
替換為您實際的部署 URL。

## 第三步：添加到個人網站

1. **選擇整合方式**
   - 打開 `personal-website-integration.html`
   - 選擇其中一個選項（推薦選項 1：簡潔卡片式）
   - 複製選中的 HTML 代碼

2. **添加到個人網站**
   - 前往個人網站的「成長領導」區塊
   - 在適當位置貼上代碼
   - 保存並發布

3. **測試**
   - 測試「了解更多」按鈕是否正確連結
   - 測試「預約體驗」按鈕是否跳轉到報名表單
   - 測試從服務網站返回個人網站的連結

## ✅ 完成檢查清單

- [ ] 網站已部署到 Vercel
- [ ] 獲得部署 URL
- [ ] 更新了整合代碼中的 URL
- [ ] 代碼已添加到個人網站
- [ ] 所有連結測試正常
- [ ] 報名表單功能正常

## 🆘 需要幫助？

如果遇到問題，請檢查：
1. GitHub repository 是否公開
2. Vercel 是否正確連接 GitHub
3. 部署 URL 是否正確更新到整合代碼中
4. 個人網站的編輯器是否支援 HTML

## 📝 備註

- 如果使用 GitHub Pages，URL 會是：`https://enya0911.github.io/self-growth-leadership`
- 可以同時使用多個部署平台（Vercel + GitHub Pages）
- 建議使用 Vercel，因為與個人網站同平台，管理更方便

