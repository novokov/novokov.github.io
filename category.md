---
layout: default
title: Categories
---

<h2 class="post-list-heading">Python</h2>
{% for post in site.categories.python %}
<ul><li><a href="{{ post.url | prepend:site.baseurl }}">{{ post.title }}</a></li></ul>
{% endfor %}

<h2 class="post-list-heading">Django</h2>
{% for post in site.categories.django %}
<ul><li><a href="{{ post.url | prepend:site.baseurl }}">{{ post.title }}</a></li></ul>
{% endfor %}

<h2 class="post-list-heading">Git</h2>
{% for post in site.categories.git %}
<ul><li><a href="{{ post.url | prepend:site.baseurl }}">{{ post.title }}</a></li></ul>
{% endfor %}

<h2 class="post-list-heading">SQL</h2>
{% for post in site.categories.sql %}
<ul><li><a href="{{ post.url | prepend:site.baseurl }}">{{ post.title }}</a></li></ul>
{% endfor %}

<h2 class="post-list-heading">SEO</h2>
{% for post in site.categories.seo %}
<ul><li><a href="{{ post.url | prepend:site.baseurl }}">{{ post.title }}</a></li></ul>
{% endfor %}

<h2 class="post-list-heading">Other</h2>
{% for post in site.categories.other %}
<ul><li><a href="{{ post.url | prepend:site.baseurl }}">{{ post.title }}</a></li></ul>
{% endfor %}


