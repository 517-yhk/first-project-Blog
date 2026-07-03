---
layout: post
title: "我的第一篇博客"
date: 2026-07-03 12:00:00 +0800
categories: 学习记录
---
前言
这是我用 GitHub Pages + Jekyll 搭建的第一篇博客，记录一下整个搭建过程和踩过的坑。

搭建过程
1. 仓库创建
首先在 GitHub 新建公开仓库，开启 GitHub Pages 功能，选择 GitHub Actions 作为构建源。

2. 本地环境配置
本地安装 Git 和 Jekyll 环境，初始化博客项目，编写基础配置文件。

3. 自动部署配置
配置 `.github/workflows` 下的工作流文件，实现代码推送后自动构建和部署。

踩过的坑
1.  **网络问题**：国内直连 GitHub 推送代码容易连接重置，给 Git 配置代理后解决。
2.  **依赖兼容**：Windows 生成的 `Gemfile.lock` 和 Linux 构建环境不兼容，删除后自动生成即可。
3.  **样式丢失**：`baseurl` 配置错误导致 CSS 加载失败，修正路径后样式正常显示。

总结
第一次用 GitHub Pages 搭建博客，虽然踩了不少坑，但最终成功上线还是很有成就感。接下来会继续更新博客，记录更多学习内容。