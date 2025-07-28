# DBSAFER POC SOP

本專案為 **DBSAFER POC SOP** 前端靜態頁面，使用 Tailwind CSS 與原生 JavaScript，並以 GitHub Pages 進行部署。

---

## 1. 專案架構
```
dbsafer-poc/
├── index.html
└── README.md
```

---

## 2. 本地預覽
直接以瀏覽器開啟 `index.html` 即可，或使用 Python 啟動簡單 HTTP 伺服器：
```bash
python -m http.server 8080
# 瀏覽 http://localhost:8080
```

---

## 3. 初始化並推送到 GitHub

```bash
git init
git add .
git commit -m "Initial commit - DBSAFER POC SOP"
git branch -M main
git remote add origin https://github.com/<your-account>/dbsafer-poc.git
git push -u origin main
```

---

## 4. 啟用 GitHub Pages

1. 進入 GitHub 專案頁面 → **Settings** → **Pages**
2. **Source** 選擇：`main` 分支、資料夾選 `/(root)`
3. 儲存後等待 1~2 分鐘，GitHub Pages 會產生你的網站 URL：  
   `https://<your-account>.github.io/dbsafer-poc/`

---

## 5. 後續維護建議
- 建議開 `gh-pages` 或 `docs` 分支作為展示用分支（若後續加入自動化 CI/CD）。
- 若未來需拆分成多頁式架構，建議導入任一前端建構工具（如 Vite）以管理資產打包。

---

© 2025 DBSAFER Inc. All Rights Reserved.
