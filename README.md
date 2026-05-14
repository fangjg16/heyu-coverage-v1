# 家办业务覆盖对比图（Heyu Coverage v1）

静态单页应用：打开 `Heyu_Coverage_v1.html` 即可使用（需与 `coverage_data.js` 同目录）。

## 本地预览

用浏览器直接打开 `Heyu_Coverage_v1.html`，或通过本地静态服务器：

```bash
npx --yes serve -p 5173
```

然后访问 `http://localhost:5173/Heyu_Coverage_v1.html`。

## 部署到 GitHub Pages

1. 在本目录初始化并推送仓库（示例仓库名 `heyu-coverage-v1`，请按需修改）：

   ```bash
   git init
   git add .
   git commit -m "Initial: 家办业务覆盖对比图"
   gh repo create heyu-coverage-v1 --public --source=. --remote=origin --push
   ```

   若未安装 [GitHub CLI](https://cli.github.com/)，可在 GitHub 网页新建空仓库后执行：

   ```bash
   git remote add origin https://github.com/<你的用户名>/heyu-coverage-v1.git
   git branch -M main
   git push -u origin main
   ```

2. 在 GitHub 仓库 **Settings → Pages** 中：
   - **Source**：Deploy from a branch  
   - **Branch**：`main` / `/ (root)`  
   - 保存后等待构建，站点地址一般为：  
     `https://<你的用户名>.github.io/heyu-coverage-v1/`  
     根路径会经 `index.html` 跳转到 `Heyu_Coverage_v1.html`。

## 仓库内容

| 文件 | 说明 |
|------|------|
| `Heyu_Coverage_v1.html` | 主页面（含样式与脚本） |
| `coverage_data.js` | 矩阵数据 |
| `index.html` | 便于 GitHub Pages 根路径跳转 |

字体与导出库仍从 Google Fonts / jsDelivr 加载，需联网。
