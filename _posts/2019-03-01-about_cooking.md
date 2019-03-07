---
layout: about
title: "Cooking!"
date: 2019-03-01
categories: About
thumbnail: "/imgs/ribs.jpg"
---
<p>
I love cooking. Here are some examples of what I cooked. 
Unfortunately, I'm not much of an Instagrammer, nor do I post my food on facebook, therefore I don't have many pictures.
</p>

{% assign filtered = site.data.images | where:"type","cook" %}

<ul>
{% for photo in filtered %}
	<div class="gallery">
	<a target="{{ photo.path }}" href="{{ photo.path }}">
    <img src="{{ photo.path }}" alt="{{ photo.short }}" width="600" height="400">
	</a>
	<div class="desc">{{photo.desc}}</div>
	</div>
{% endfor %}
</ul>