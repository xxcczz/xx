---
layout: default
title: My Blog
---
{% for post in paginator.posts %}
    <a href="{{ \xx{{ post.url }} }}">{{ post.title }}</a>
{% endfor %}