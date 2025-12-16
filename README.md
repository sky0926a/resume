# Jimmy Li - Bilingual Senior Software Engineer Resume

一個現代化的雙語履歷網頁，專為後端資深工程師職位設計，支援網頁互動版與 A4 列印列版。

## 🚀 特色

- **雙語支援**：完整支援繁體中文 (Traditional Chinese) 與英文 (English)
- **列印最佳化**：提供專為 A4 紙張設計的列印版 (Print-friendly versions)
- **現代深色主題**：優雅的漸層配色和玻璃擬態效果
- **動態互動**：打字效果、滾動動畫、視差效果
- **完全響應式**：支援桌面、平板和手機裝置
- **效能優化**：使用 Intersection Observer 進行懶載入
- **無框架依賴**：純 HTML、CSS、JavaScript 實作

## 📁 檔案結構

```
resume/
├── index.html           # [中文] 網頁版履歷 (預設首頁)
├── index-en.html        # [英文] 網頁版履歷
├── resume-print.html    # [中文] 列印版履歷 (A4 最佳化)
├── resume-print-en.html # [英文] 列印版履歷 (A4 最佳化)
├── styles.css           # 網頁版共用樣式
├── script.js            # 網頁版互動邏輯
└── README.md            # 說明文件
```

> **注意**：`resume-print*.html` 檔案內含獨立 CSS 樣式，不依賴 `styles.css`，以確保列印樣式的一致性。

## 🌐 部署到 GitHub Pages

### 方法一：使用 GitHub 網頁介面

1. 建立新的 GitHub Repository（例如：`username.github.io` 或 `resume`）
2. 上傳所有檔案到 Repository
3. 前往 **Settings** > **Pages**
4. 在 **Source** 選擇 `main` branch
5. 點擊 **Save**
6. 等待幾分鐘後，訪問 `https://username.github.io/resume/`

### 方法二：使用 Git 命令列

```bash
# 初始化 Git repository
git init

# 添加所有檔案
git add .

# 提交變更
git commit -m "Initial commit: Add bilingual resume website"

# 添加遠端 repository (替換 YOUR_USERNAME)
git remote add origin https://github.com/YOUR_USERNAME/resume.git

# 推送到 GitHub
git push -u origin main
```

然後在 GitHub Repository Settings 中啟用 GitHub Pages。

## 📝 自訂內容

由於本專案包含雙語及列印版，修改內容時請確保 **同時更新** 以下檔案：

1. `index.html` (中文網頁)
2. `index-en.html` (英文網頁)
3. `resume-print.html` (中文列印)
4. `resume-print-en.html` (英文列印)

### 主要修改區塊

- **Hero Section**: 姓名、職稱、聯絡方式
- **About/Summary**: 個人簡介
- **Experience**: 工作經歷
- **Skills**: 技術技能
- **Projects**: 專案作品
- **Education**: 學歷背景

### 修改樣式

網頁版樣式位於 `styles.css`：

```css
:root {
    --accent-primary: #6366f1;     /* 主要強調色 */
    --accent-secondary: #8b5cf6;   /* 次要強調色 */
    /* ... 其他變數 */
}
```

列印版樣式直接位於 html 檔案的 `<style>` 標籤內。

## 💡 效能建議

- 所有圖片使用 WebP 格式
- 使用 CDN 載入字型
- 啟用 GZIP 壓縮
- 考慮使用 Service Worker 進行離線快取

## 📧 聯絡方式

如有任何問題，歡迎開 Issue 或 Pull Request！

---

Built with ❤️ by Jimmy Li
