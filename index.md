---
layout: page
title: Notas sobre problemas del Proyecto euler
tagline: projecteuler.net
---
{% include JB/setup %}

{% highlight julia linenos %}
for k in range(1000000):
	EsPrimo(k)
{% endhighlight %}


## Entradas:
<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

