---
layout: page
title: Notas sobre problemas del Proyecto euler
tagline: projecteuler.net
---
{% include JB/setup %}

## Entradas:
<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

{% gist e9bc06d7b79aa3dc275d}
