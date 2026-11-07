# 好物算算 · 日常消耗品单价追踪与智能比价

T-020 轻应用（v1.1）静态站点版。单文件 H5，无后端；数据存在浏览器 localStorage。

## 本地预览
直接双击 `index.html`，或：

```bash
python3 -m http.server 8787
```

然后打开 http://127.0.0.1:8787/

## 部署到 GitHub Pages
1. 新建仓库（如 `what-to-buy`），把本目录内容推到 `main` 分支根目录。
2. 仓库 Settings → Pages → Source 选 `Deploy from a branch`，Branch 选 `main` / `(root)`，保存。
3. 约 1 分钟后访问 `https://<用户名>.github.io/<仓库名>/`。

## 说明
- ECharts 走 CDN；CDN 不可达时自动降级为内联 SVG 图表。
- 飞书 Bitable 默认 Mock 适配器；真实联调需在「设置」里填 App ID/Secret 与代理基址（凭证只存本机 localStorage）。
