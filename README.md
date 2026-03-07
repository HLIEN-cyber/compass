# COMPASS GitHub Pages 部署說明

此專案為純靜態網站，首頁檔案為 `index.html`。

## 自動部署（GitHub Actions）

已提供 workflow：`.github/workflows/deploy.yml`。

觸發條件：
- push 到 `main` 或 `master`
- 手動觸發（workflow_dispatch）

## 第一次啟用 Pages 必做

1. 到 GitHub repository → **Settings** → **Pages**。
2. 在 **Build and deployment** 中，Source 選擇 **GitHub Actions**。
3. 之後每次 push 到主分支就會自動部署。

## 本機預覽

```bash
python3 -m http.server 8000
```

打開：<http://127.0.0.1:8000>
