---
layout: default
title: Categories
---

<h2 class="post-list-heading">Django</h2>

<ul class="post-list">
{% for post in site.categories.django %}
	
	<li><a href="{{ post.url | prepend:site.baseurl }}">{{ post.title }}</a></li>

{% endfor %}
</ul>

<h2 class="post-list-heading">Other</h2>

<ul class="post-list">
{% for post in site.categories.other %}
	
	<li><a href="{{ post.url | prepend:site.baseurl }}">{{ post.title }}</a></li>

{% endfor %}
</ul>



<a href="https://www.youtube.com/watch?v=pe4LxyK_hPo&list=PLyHuZVg03hQjtV45HPlfuPzHJOtEoK6DT&index=5" rel="nofollow">ссылка на гайд</a>
