# AI 推歌评估 · 静态网页

单文件 HTML 页面，采用浅色界面，原生 CSS 和 JavaScript，无需后端、数据库或 npm 构建。

## 本地使用

直接用浏览器打开 `index.html`，或在本目录运行 `python3 -m http.server 8000`，浏览器访问 `http://localhost:8000/`。

## GitHub Pages 部署

1. 在 GitHub 创建公开仓库，例如 `ai-music-eval-static`。
2. 将 `index.html` 和 `README.md` 提交到默认分支根目录。
3. 打开 Settings → Pages，选择 Deploy from a branch，选择 `main` 和 `/ (root)`，保存。
4. 部署完成后，通过 `https://<github-username>.github.io/ai-music-eval-static/` 访问。

## 范围说明

- 页面使用一条提供的音乐推荐结果，追加两轮交互占位数据供按钮切换。
- 默认模型评分数值为静态占位数据，不代表已运行 LLM Judge。
- 人工分数和确认状态只在页面运行期间保留，刷新后重置。
- 复制评分记录需要浏览器支持剪贴板权限；建议通过 localhost 或 HTTPS 访问。
- 所有曲目信息为前端呈现，不含需要鉴权的过期播放 URL。
