---
layout: default
title: Galeria
permalink: /fotos/
lightbox: true

---

<header  id="page-header" class="carta-header anm-moveFromTop">
	<div>
		<h1 class="anm-moveFromBottomFade delay-100">{{ page.title }}</h1>
	</div>
</header>
<main id="page-main" role="main">
	<div id="layout" class="listed">
    	<h3 class="anm-moveFromLeftFade delay-500"><u>El Centro Médico</u></h3>
		<section class="anm-fadeIn delay-500">					
	{% assign image_files = site.static_files | where: "image", true %}
	{% for image in image_files %}
	<article>
    	<a href="{{ site.baseurl }}/assets/bio/{{ image.name }}" data-lightbox="roadtrip"><img class="imagens" src="{{ site.baseurl }}/assets/bio	/{{ image.name }}" alt="El centro médico"></a>
	</article>
	{% endfor %}
		</section>
	<hr>
	</div><!-- /#Layout -->
</main>
