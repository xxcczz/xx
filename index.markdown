---
layout: default
title: 阿呆
---
<p>
文章总数:{{ paginator.total_posts }}
</p>
  <ul class="posts">
    {% for post in site.posts %}
      <li><a href="\xx{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>