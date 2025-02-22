---
layout: default
title: 文章列表
pagination: true
---

{% for post in paginator.posts %}
- [{{ post.title }}]({{ post.url }}) ({{ post.date | date: "%Y-%m-%d" }})
{% endfor %}

<!-- 分頁導航 -->
<div>
  {% if paginator.previous_page %}
    <a href="{{ paginator.previous_page_path }}">« 上一頁</a>
  {% endif %}
  {% if paginator.next_page %}
    <a href="{{ paginator.next_page_path }}">下一頁 »</a>
  {% endif %}
</div>
