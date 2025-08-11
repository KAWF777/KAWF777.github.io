---
layout: default
title: 分类目录
---

<h2>文章分类</h2>
{% for category in site.categories %}
<h3 id="{{ category[0] }}">{{ category[0] }}</h3>
<ul>
  {% for post in category[1] %}
  <li><a href="{{ post.url | relative_url }}">{{ post.title }}</a> ({{ post.date | date: '%Y-%m-%d' }})</li>
  {% endfor %}
</ul>
{% endfor %}
