---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults
title: Ateliê Raissa Moura
layout: default
---

<div>
	<h2>Obras disponíveis</h2>
	{% assign disponiveis = site.posts | where: "categories", "disponivel" %}
{% for post in disponiveis %}
<div class="row p-3">      
<img src="{{post.image}}" alt="{{post.title}}" class="col-3 img-thumbnail" style="border: none;"/>
<div class="col-9">
	<h3>{{ post.title }}</h3>
	
{{ post.excerpt }}</div>
</div>

{% endfor %}

</div>

<div>
	<h2>Obras indisponíveis</h2>
	{% assign indisponiveis = site.posts | where: "categories", "indisponivel" %}
{% for post in indisponiveis %}
<div class="row p-3">      
<img src="{{post.image}}" alt="{{post.title}}" class="col-3 img-thumbnail" style="border: none;"/>
<div class="col-9">
	<h3>{{ post.title }}</h3>
	
{{ post.excerpt }}</div>
</div>

{% endfor %}

</div>
