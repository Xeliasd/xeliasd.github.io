---
layout: about
title: "Gardening"
date: 2019-03-01
categories: About
thumbnail: "/imgs/kalerab.jpg"
---
I like gardening, it brings peace of mind while also being a quite good way to stay in shape. 
In recent years I unfortunately do not have much time for visiting my old garden, so I ttry to grow at least some herbs on my balcony.

<ul>
{% for photo in site.data.images %}
	{% if photo.type == "garden" %}
	<div class="gallery">
	<a target="{{ photo.path }}" href="{{ photo.path }}">
    <img src="{{ photo.path }}" alt="{{ photo.short }}" width="600" height="400">
	</a>
	<div class="desc">{{photo.desc}}</div>
	</div>
	{% endif %}
{% endfor %}
</ul>
