---
layout: post
title: 如何使用 GitHub Pages 搭建个人博客
date: 2026-01-08 11:00:00 +0800
categories: [教程, Jekyll]
---

GitHub Pages 是 GitHub 提供的静态网页托管服务，非常适合用来搭建个人博客。本文将介绍如何从零开始搭建一个美观的个人博客。

## 什么是 GitHub Pages

GitHub Pages 是一项免费服务，可以直接从 GitHub 仓库托管静态网站。它支持：

- Jekyll 静态网站生成器
- 自定义域名
- HTTPS 支持
- 无限流量

## 创建步骤

### 1. 创建仓库

在 GitHub 上创建一个新仓库，命名为 `your-username.github.io`，其中 `your-username` 是你的 GitHub 用户名。

### 2. 克隆仓库

```bash
git clone https://github.com/your-username/your-username.github.io.git
cd your-username.github.io
```

### 3. 创建配置文件

创建 `_config.yml` 文件，配置博客的基本信息：

```yaml
title: 我的博客
description: 个人技术博客
author: 你的名字
```

### 4. 创建目录结构

```
.
├── _config.yml       # 配置文件
├── _layouts/         # 布局模板
├── _posts/          # 博客文章
├── assets/          # 静态资源
│   └── css/         # 样式文件
└── index.html       # 首页
```

### 5. 编写文章

在 `_posts` 目录下创建 Markdown 文件，文件名格式为 `YYYY-MM-DD-标题.md`。

### 6. 推送到 GitHub

```bash
git add .
git commit -m "Initial commit"
git push origin main
```

## 访问你的博客

几分钟后，访问 `https://your-username.github.io` 就能看到你的博客了！

## 自定义主题

你可以：

1. 使用 Jekyll 主题（如 Minima）
2. 自己设计样式
3. 使用第三方主题

## 总结

GitHub Pages 是搭建个人博客的绝佳选择，免费、稳定、易于使用。赶快动手试试吧！

> 提示：如果你想使用自定义域名，只需要在仓库根目录创建一个 `CNAME` 文件，填入你的域名即可。
