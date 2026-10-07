# Principles of Modern Chemistry · 目录浏览与智能检索

《Principles of Modern Chemistry》(7th Edition) 的网页版目录与阅读器，可直接在手机浏览器中打开，无需 PDF 插件。

## 功能

- **目录浏览**：按 Unit → Chapter → 小节 三级展开，支持关键词搜索与高亮
- **作业分区**：每个小节的作业习题在目录中单独成条（琥珀色「作业」标签），与正文分开
- **阅读器**：书页以图片呈现，支持左右滑动翻页、双击放大、缩放按钮、上一节/下一节
- **断点续读**：自动记住上次阅读的页码与位置

## 目录结构

```
.
├── index.html      # 单文件应用（目录 + 阅读器）
├── .nojekyll       # 关闭 Jekyll 处理，加快 Pages 构建
└── pages/          # 书页图片，0001.webp ~ 1288.webp（120 DPI WebP）
```

## 关于 AI 检索

本站为**纯静态版本**，不包含 AI 辅助检索功能（该功能依赖服务器端的 Node 接口与 GLM 模型调用）。
带 AI 检索的版本部署在服务器上，如需该功能请使用服务器版。

## 本地预览

```bash
python -m http.server 8080
# 打开 http://localhost:8080/
```

## 更新书页

替换 `pages/` 目录下的 WebP 图片后重新提交即可，文件名需保持 `0001.webp` ~ `1288.webp` 的补零格式。