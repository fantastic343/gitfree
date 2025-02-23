---
layout: default
title: 首頁
---

# 歡迎來到gitfree

這裡是一個提供 **獨立、客觀** 觀點與深度思考的空間。我們關注 **社會、科技、哲學、時事** 等議題，鼓勵批判性思考與理性討論。  

## 📌 最新文章  
{% for post in site.posts limit:5 %}
- [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%Y-%m-%d" }}
{% endfor %}

## 🔥 推薦閱讀  
- [翻牆軟體下載](./vpn.md)  
- [科技如何影響未來社會？](./future.md)  
- [哲學與日常：如何理性決策](./philosophy.md)  
