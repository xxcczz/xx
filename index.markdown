---
layout: default
title: 阿呆
---
  <ul class="posts">
    {% for post in site.posts %}
      <li><a href="\xx{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
	
	{% for post in paginator.posts %}
<article class="excerpt excerpt-c5">
    <a class="thumbnail" href={{ post.url }}>
        <img src="/assets/images/cover.jpg" class="thumb" style="display: inline;">
    </a>
    <h2>
        <a href={{ post.url }}>{{ post.title | strip_html | strip_newlines | truncate: 250 }}&hellip;
        </a>
    </h2>
    <footer>
        <a href="javascript:;" class="post-like" data-pid="135" etap="like">
            <i class="fa"></i><span>&chi;</span>
        </a>
        <time class="hot">Hot</time>
        <span class="post-view">{{ post.date | date: "%F"}}</span>
        <span class="post-comm">{{ post.tags }}</span>
    </footer>
</article>
{% endfor %}
{% include pagination.html %}