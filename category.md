---
layout: default
title: category
---

{% for post in site.categories.django %}
	
	{{ post.title }}<br><hr>

{% endfor %}


