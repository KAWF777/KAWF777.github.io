# koon的博客

网址：https://kawf777.github.io

基于 Jekyll 与 GitHub Pages 的文字博客，无需付费服务器或域名。保留原始文章与链接。包含首页、文章页、归档、关于、RSS 和 404 页面，适配手机。

## 发布文章

在 GitHub 打开 `_posts`，选择 Add file → Create new file。文件名使用 `年-月-日-英文短标题.md`，例如 `2026-09-05-a-new-day.md`。内容示例：

```markdown
---
layout: post
title: "在这里写标题"
date: 2026-09-05
categories: [随笔]
---

第一段文字会成为首页摘要。

<!--more-->

这里继续写正文。支持 Markdown 标题、列表、链接和图片。
```

提交到 main 后 GitHub Pages 会自动更新，通常需要几分钟。不要使用未来日期，否则文章会等到该日期才显示。图片可以放进 `assets/img`。

## 修改博客

- `_config.yml`：名称、简介、网址。
- `about.html`：关于页面。
- `assets/css/style.css`：字体、颜色和排版。
- `_layouts/post.html`：文章结构与回复占位区。

## 回复功能

第一版仅为界面占位：文本框和按钮均为原生 disabled 状态，无提交接口，不收集、保存或发送回复。后续可接入评论服务；届时需要单独配置存储、身份验证与隐私说明，不能只移除 disabled。

## 部署与维护

GitHub 仓库 Settings → Pages 使用 Deploy from a branch，选择 main 和 /(root)。保留 Jekyll 构建，勿添加 `.nojekyll`。代码和文章均位于公开仓库；请勿提交密码或私人资料。

原有 `categories.md` 分类入口及文章 URL 保持兼容。旧背景素材保留，但新版不使用它们。
