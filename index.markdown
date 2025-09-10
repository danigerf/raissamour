---
title: Ateliê Raissa Moura
layout: default
---

<div>
	<!-- <h2>Obras disponíveis</h2> -->

<div class='row mt-3' data-masonry='{"percentPosition": true }' id="gallery">
{% for post in site.posts %}
<div class="col-sm-6 col-lg-4 mb-4">
	<a href="{{post.url}}">

<img src="{{post.image}}" alt="{{post.title}}" class="img-fluid rounded" style="border: none;"/>

</a>

</div>
{% endfor %}

</div>
</div>
