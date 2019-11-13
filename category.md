---
layout: default
title: Categories
---

<h2 class="post-list-heading">Python</h2>

{% for post in site.categories.python %}
	- <a href="{{ post.url | prepend:site.baseurl }}">{{ post.title }}</a>
{% endfor %}

<h2 class="post-list-heading">Django</h2>
{% for post in site.categories.django %}
	- <a href="{{ post.url | prepend:site.baseurl }}">{{ post.title }}</a>
{% endfor %}

<h2 class="post-list-heading">Git</h2>
<ul class="post-list">
{% for post in site.categories.git %}
	- <a href="{{ post.url | prepend:site.baseurl }}">{{ post.title }}</a>
{% endfor %}
</ul>

<h2 class="post-list-heading">SQL</h2>
<ul class="post-list">
{% for post in site.categories.sql %}
	- <a href="{{ post.url | prepend:site.baseurl }}">{{ post.title }}</a>
{% endfor %}
</ul>

<h2 class="post-list-heading">SEO</h2>
<ul class="post-list">
{% for post in site.categories.seo %}
	<li><a href="{{ post.url | prepend:site.baseurl }}">{{ post.title }}</a></li>
{% endfor %}
</ul>

<h2 class="post-list-heading">Other</h2>
<ul class="post-list">
{% for post in site.categories.other %}
	<li><a href="{{ post.url | prepend:site.baseurl }}">{{ post.title }}</a></li>
{% endfor %}
</ul>


