---
layout: page
title: "博客文章"
permalink: /blog/
---

# 博客文章

这里是我所有的技术博客文章，按时间倒序排列。

## 文章列表

{% for post in site.posts %}
### {{ post.date | date: "%Y年%m月%d日" }} · [{{ post.title }}]({{ post.url }})

**分类**：{{ post.categories | join: ", " }}  
**标签**：{{ post.tags | join: ", " }}

{{ post.excerpt | strip_html | truncate: 200 }}

[阅读全文 →]({{ post.url }})
{% endfor %}

## 分类浏览

{% for category in site.categories %}
### {{ category[0] }}
{% for post in category[1] limit:3 %}
- [{{ post.title }}]({{ post.url }}) ({{ post.date | date: "%Y-%m-%d" }})
{% endfor %}
{% endfor %}

## 标签云

{% assign tags = site.tags | sort %}
{% for tag in tags %}
[#{{ tag[0] }}](/tags/{{ tag[0] }}) 
{% endfor %}

---

*文章总数量：{{ site.posts | size }} 篇*  
*最后更新时间：{{ site.time | date: "%Y年%m月%d日 %H:%M" }}*
