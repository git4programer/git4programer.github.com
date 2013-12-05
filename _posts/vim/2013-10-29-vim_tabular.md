---
layout: default
title: "vim tabular插件"
description: "vim tabular"
category: "vim"
tags: [vim,vim插件]
---
{% include JB/setup %}


## vim tabular插件

vim tabular插件是一个让一些文本的特定的对齐插件，如下面


	$goods_id =$_POST['goods_id'];
	$goods_name = $_POST['goods_name'];
	$goods_class = $_POST['goods_class'];
	$goods_number = $_POST['goods_number']

	$goods_id     = $_POST['goods_id'];
	$goods_name   = $_POST['goods_name'];
	$goods_class  = $_POST['goods_class'];
	$goods_number = $_POST['goods_number']


上面的代码如果想格式化为下面那种的对齐方式，你只需要把光标移到要对齐的行上面，然后进入命令行的模式


	:Tab /= 


就可以实现了,注意到那命令的格式，要按照＝对齐就是 :Tab/=,那我大胆的假设一下，只要输入这个命令就会按照后面的那个字符对齐的。于是我做了下在的测试


	abcccccc   d fggggggg
	a          d ffffggggh
	bfwerefgkj d s         d kfjjk


我输入了


	:Tab /d


果然它就按照d来对齐了，而且d的两边都有一个空格!!
