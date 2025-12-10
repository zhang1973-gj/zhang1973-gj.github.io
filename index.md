---
layout: home  # 关联你之前的home.html布局（也可以用default）
title: 我的测试博客
---

测试配置

[首页](/)[关于](/about/)[归档](/archive/)

# 你好!
这是我的个人博客，使用GitHub Pages搭建。

## 最新文章
{% if site.posts.size > 0 %}
  <ul>
    {% for post in site.posts %}
      <li>
        <a href="{{ post.url }}">{{ post.title }}</a>
        <small>{{ post.date | date: "%Y年%m月%d日" }}</small>
      </li>
    {% endfor %}
  </ul>
{% else %}
  <p>暂无文章，快来写第一篇吧！</p>
{% endif %}

欢迎常来看看!
