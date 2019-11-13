---
layout: default
title: Categories
---

{% for post in site.categories.django %}
	
	<a href="{{ post.url | prepend:site.baseurl }}">{{ post.title }}</a>

{% endfor %}

<a href="https://www.youtube.com/watch?v=pe4LxyK_hPo&list=PLyHuZVg03hQjtV45HPlfuPzHJOtEoK6DT&index=5" rel="nofollow">ссылка на гайд</a>
