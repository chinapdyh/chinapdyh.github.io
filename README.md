# GaussianArtist - 3DGS 技术博客

这是我的个人技术博客，专注于 3D 高斯溅射（3D Gaussian Splatting）、点云渲染、计算机图形学技术分享。

## 博客地址

🔗 **在线访问**: [https://chinapdyh.github.io](https://chinapdyh.github.io)

## 技术栈

- **静态站点生成器**: Jekyll 4.3.2
- **主题**: Minima 2.5
- **托管平台**: GitHub Pages
- **CI/CD**: GitHub Pages 自动构建

## 本地开发

### 环境要求
- Ruby 2.6.0+
- Bundler gem

### 安装步骤
```bash
# 克隆仓库
git clone https://github.com/chinapdyh/chinapdyh.github.io.git
cd chinapdyh.github.io

# 安装依赖
bundle install

# 启动本地服务器
bundle exec jekyll serve
```

然后访问 http://localhost:4000 查看博客。

### 新建文章
```bash
# 在 _posts 目录下创建新的 Markdown 文件
# 文件名格式: YYYY-MM-DD-title.md
```

### 文章 Front Matter 模板
```yaml
---
layout: post
title: "文章标题"
date: 2024-03-23 18:00:00 +0800
categories: [分类1, 分类2]
tags: [标签1, 标签2, 标签3]
author: GaussianArtist
---
```

## 项目结构

```
.
├── _config.yml          # Jekyll 配置文件
├── _posts/              # 博客文章目录
│   └── 2024-03-23-3DGS-PLY-rendering-basics.md
├── index.md             # 主页
├── about.md             # 关于页面
├── blog.md              # 博客文章列表
├── Gemfile              # Ruby 依赖配置
└── README.md            # 项目说明
```

## 文章分类

- **3DGS**: 3D 高斯溅射技术
- **点云渲染**: 点云数据处理和渲染
- **Unity**: Unity 3D 图形编程
- **计算机图形学**: 基础理论和算法

## 部署

博客自动通过 GitHub Pages 部署。每次推送到 `main` 分支时，GitHub 会自动构建并发布站点。

### 手动构建
```bash
# 生成静态文件到 _site 目录
bundle exec jekyll build
```

## 许可证

博客内容采用 [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) 许可证。

代码部分采用 MIT 许可证。

## 联系

- GitHub: [@chinapdyh](https://github.com/chinapdyh)
- 博客: [chinapdyh.github.io](https://chinapdyh.github.io)

---
*最后更新: {{ site.time | date: "%Y年%m月%d日" }}*
