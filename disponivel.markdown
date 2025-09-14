---
title: Obras Disponíveis
layout: default
---

  <div class="row grid d-block mx-auto" data-masonry='{"percentPosition": true }'>
  
    {% for post in site.categories.disponivel %}
		<div class="col-sm-6 col-lg-4 mb-4 grid-item text-center d-block">
		
		<a href="{{post.url}}" class="">
			<img src="{{post.image}}" alt="{{post.title}}" class="img-fluid rounded mx-auto d-block" style="border: none;"/>
		</a>
		
		</div>
    {% endfor %}
  </div>
