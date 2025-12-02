# 整合到個人網站指南

## 方案一：獨立部署後連結（推薦）

### 步驟 1：部署自我成長領導力網站

如果還沒有部署，可以使用以下方式：

#### 使用 Vercel（與個人網站相同平台）

```bash
# 安裝 Vercel CLI（如果還沒有）
npm install -g vercel

# 在專案目錄執行
cd /Users/samuelhou/self-growth-leadership
vercel

# 生產環境部署
vercel --prod
```

部署後會獲得一個 URL，例如：`https://self-growth-leadership.vercel.app`

#### 或使用 GitHub Pages

網站已經在 GitHub 上，可以啟用 GitHub Pages：
- Repository: `enya0911/self-growth-leadership`
- GitHub Pages URL: `https://enya0911.github.io/self-growth-leadership`

### 步驟 2：在個人網站中添加連結

在個人網站的「成長領導」區塊中，可以添加：

```html
<!-- 在「成長領導」區塊中添加 -->
<div class="service-card">
  <h3>自我成長領導力</h3>
  <p>透過深度提問、結構化成長計畫與情緒覺察，陪你走向更成熟穩定的自我成長領導力。</p>
  <a href="https://self-growth-leadership.vercel.app" target="_blank" class="btn-primary">
    了解更多 →
  </a>
</div>
```

## 方案二：嵌入到個人網站中

如果需要將內容直接嵌入到個人網站，可以：

1. 將 `index.html` 的內容提取為一個組件
2. 在個人網站的「成長領導」頁面中嵌入
3. 調整樣式以避免衝突

## 方案三：添加返回個人網站的連結

在自我成長領導力網站中添加返回個人網站的連結：

在 navbar 或 footer 中添加：
```html
<a href="https://personal-website-8939.vercel.app" class="back-link">
  ← 返回個人網站
</a>
```

## 建議的整合方式

**推薦使用方案一**，因為：
1. 保持兩個網站的獨立性
2. 更好的 SEO 和性能
3. 更容易維護和更新
4. 用戶體驗更好（專注的 landing page）

在個人網站的「成長領導」區塊中，可以這樣呈現：

```
🧂 自我成長領導力

透過深度提問、結構化成長計畫與情緒覺察，陪你走向更成熟穩定的自我成長領導力。

[了解更多] [預約體驗]
```

兩個按鈕分別連結到：
- 了解更多：完整的 landing page
- 預約體驗：直接打開報名表單（可以在 URL 中添加 #cta 錨點）

