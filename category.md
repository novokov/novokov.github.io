---
layout: default
title: Categories
---

{% for post in site.categories.django %}
	
	{{ post.title }}<br><hr>

{% endfor %}


