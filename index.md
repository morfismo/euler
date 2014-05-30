---
layout: page
title: Notas sobre problemas del Proyecto euler
tagline: projecteuler.net
---
{% include JB/setup %}

{% highlight julia linenos %}
function EsPrimo(n)
	MX=1000
	if (n <= MX) # Si el número es menor o igual que MX
		if (n in ListaPrimos)  # Basta con verificar pertenencia
			return true
		else
			return false
		end   
	elseif (MX < n) &&  (n<=MX*MX)  # Si el número está entre MX y MX^2
		for p in ListaPrimos
			( n%p == 0 ) && return false  # Si alguno divide, no es primo
			( p>n*n) && return true
		end
		return true
	else
		println("Fuera de Rango!", MX, n, MX*MX)
		return false
	end
end


{% endhighlight %}

$$x^2 + y^2 = z^2$$

$$\sqrt{\cos{\pi x}}$$.

## Entradas:
<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

