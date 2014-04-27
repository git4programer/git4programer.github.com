---
layout : default
title : kasonpasser
---
{% include JB/setup %}

<div class="col-lg-9">

<h2> 文章列表</h2>
<ul>
{% for post in site.posts %}
<li>{{ post.date | date_to_string }} <a href="{{ site.production_url }}{{ post.url }}">{{ post.title }}</a> </li>
{% endfor %}

</ul>
</div>
<div class="col-lg-3">
	<div>
	<h3>分类</h3>
	{% for category in site.categories %} 
	<h4 id="{{ category[0] }}-ref">{{ category[0] | join: "/" }}</h4>
	<ul>
	{% assign pages_list = category[1] %}  
	{% include JB/pages_list %}
	</ul>
	{% endfor %}
	</div>

	<div>
	<h3>标签</h3>
	<ul class="tag_box inline">
	  {% assign tags_list = site.tags %}  
	  {% include JB/tags_list %}
	</ul>
	</div>

	<div>
	<h3>Archive</h3>
	{% assign posts_collate = site.posts %}
	{% include JB/posts_collate %}
	</div>
</div>

