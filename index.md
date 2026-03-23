---
layout: home
title: "GaussianArtist - 3DGS 技术博客"
description: "分享3D高斯溅射、点云渲染、计算机图形学技术"
---

# 欢迎来到 GaussianArtist 技术博客！

这里是我学习和分享 3D 高斯溅射（3D Gaussian Splatting）技术的空间。

## 关于我

我是 GaussianArtist，一名对计算机图形学和 3D 渲染技术充满热情的开发者。专注于 3DGS、点云渲染、实时图形技术。

## 最新文章

{% for post in site.posts limit:5 %}
### [{{ post.title }}]({{ post.url }})
*{{ post.date | date: "%Y年%m月%d日" }}* · {{ post.categories | join: ", " }}

{{ post.excerpt | strip_html | truncate: 150 }}
{% endfor %}

[查看所有文章 →](/blog.html)

## 技术栈

- **3D 高斯溅射（3DGS）**
- **点云渲染和可视化**
- **Unity 和 C# 图形编程**
- **PLY 格式解析与处理**
- **GPU 计算与优化**
- **计算机图形学基础**

## 项目

### 当前项目
- **3DGS Unity 渲染器**：从零实现的 3DGS 点云加载、渲染和优化
- **PLY 解析工具**：高性能的 PLY 文件读取和转换工具
- **点云可视化系统**：支持百万级点云的实时渲染

### 计划项目
- GPU Instancing 优化
- 实时 3DGS 渲染管线
- Web 端 3DGS 可视化

## 联系我

- GitHub: [@chinapdyh](https://github.com/chinapdyh)
- 博客: [chinapdyh.github.io](https://chinapdyh.github.io)

---

*这个博客使用 Jekyll 构建，托管在 GitHub Pages。*
*主题使用 Minima，支持响应式设计。*
