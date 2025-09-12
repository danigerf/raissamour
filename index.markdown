---
title: Ateliê Raissa Moura
layout: default
---



  <div class="grid mx-auto" data-masonry='{"percentPosition": true }'>
  
    {% for post in site.categories.disponivel %}
		<div class="col-sm-6 col-lg-4 mb-4 grid-item text-center">
		
		<a href="{{post.url}}">
			<img src="{{post.image}}" alt="{{post.title}}" class="img-fluid rounded" style="border: none;"/>
		</a>
		
		</div>
    {% endfor %}
  </div>