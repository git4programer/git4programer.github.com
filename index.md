---
layout : default
title : git4programer的个人博客
---
{% include JB/setup %}

{% for post in site.related_posts %}
# {{ post.title }}
#### {{ post.date | date_to_string }} | {{ post.author }}

{{ post.content }}

{% endfor %}

## 文章列表
<ul>
	{% for post in site.posts %}
	<li>{{ post.date | date_to_string }} <a href="{{ site.production_url }}{{ post.url }}">{{ post.title }}</a> </li>
	{% endfor %}

</ul>
