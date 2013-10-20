---
layout : default
title : git4programer的个人博客
---


#git help
###git 放弃最新修改的内容.
git throwh

##git stash隐藏修改
中间这间可以做任何的修改
git stash apply 把隐藏的取出来.

###删除分支
git branch -D 分支号 
###创建fasdfdf版本号的分支
git checkout fasdfdf -b 分支号

## 文章列表
<ul>
	{% for post in site.posts %}
	<li>{{ post.date | date_to_string}} <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a> </li>
	{% endfor %}

</ul>
