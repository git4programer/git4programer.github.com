---
layout: default
title: "linux下面的快捷键"
description: "linux下面的快捷键"
category: "linux"
tags: [linux，快捷键]
---


# linux的快捷键


在命令行下的的快捷键：

## 删除
	ctrl + d      //删除光标所在位置上的字符相当于VIM里x或者dl
	ctrl + h      //删除光标所在位置前的字符相当于VIM里hx或者dh
	ctrl + k      //删除光标后面所有字符相当于VIM里d shift+$
	ctrl + u      //删除光标前面所有字符相当于VIM里d shift+^
	ctrl + w      //删除光标前一个单词相当于VIM里db
	ctrl + y      //恢复ctrl+u上次执行时删除的字符
	ctrl + ?      //撤消前一次输入
	alt  + r      //撤消前一次动作
	alt  + d      //删除光标所在位置的后单词

## 移动
	ctrl + a			   //将光标移动到命令行开头相当于VIM里shift+^
	ctrl + e			   //将光标移动到命令行结尾处相当于VIM里shift+$
	ctrl + f			   //光标向后移动一个字符相当于VIM里l
	ctrl + b			   //光标向前移动一个字符相当于VIM里h
	ctrl + 方向键左键     //光标移动到前一个单词开头
	ctrl + 方向键右键     //光标移动到后一个单词结尾
	ctrl + x       	   //在上次光标所在字符和当前光标所在字符之间跳转
	alt  + f      		   //跳到光标所在位置单词尾部

## 替换
	ctrl + t       //将光标当前字符与前面一个字符替换
	alt  + t       //交换两个光标当前所处位置单词和光标前一个单词
	alt  + u       //把光标当前位置单词变为大写
	alt  + l       //把光标当前位置单词变为小写
	alt  + c       //把光标当前位置单词头一个字母变为大写

## 历史命令编辑
	ctrl + p       //返回上一次输入命令字符
	ctrl + r       //输入单词搜索历史命令
	alt  + p       //输入字符查找与字符相接近的历史命令

## 其它
	ctrl + s      //锁住终端
	ctrl + q      //解锁终端
	ctrl + l      //清屏相当于命令clear
	ctrl + c      //另起一行
	ctrl + i      //类似TAB健补全功能
	ctrl + o      //重复执行命令
	alt  + 数字键 //操作的次数



# VIM下的快捷键：

###复制、删除：

yw 表示拷贝从当前光标到光标所在单词结尾的内容.

　　dw 表示删除从当前光标到光标所在单词结尾的内容.

　　y0 表示拷贝从当前光标到光标所在行首的内容.

　　d0 表示删除从当前光标到光标所在行首的内容.

　　y$ 表示拷贝从当前光标到光标所在行尾的内容.

d$ 表示删除从当前光标到光标所在行尾的内容.

移动：

    w(e) 移动光标到下一个单词.
　　b 移动光标到上一个单词.
　　0 移动光标到本行最开头.
　　^ 移动光标到本行最开头的字符处.
　　$ 移动光标到本行结尾处.
　　H 移动光标到屏幕的首行.
　　M 移动光标到屏幕的中间一行.
　　L 移动光标到屏幕的尾行.
　　gg 移动光标到文档首行.
　　G 移动光标到文档尾行.

## 常用：

	H ：光标移至屏幕顶行
	M ：光标移至屏幕中间行
	L ：光标移至屏幕最后行
	0：（注意是数字零）光标移至当前行首
	$：光标移至当前行尾

	w或W ：光标右移一个字至字首
	b或B ：光标左移一个字至字首
	e或E ：光标右移一个字至字尾
	Ctrl+u：向文件首翻半屏
	Ctrl+d：向文件尾翻半屏
	Ctrl+f：向文件尾翻一屏
	Ctrl＋b；向文件首翻一屏

	i ：在光标前
	I ：在当前行首
	a：光标后
	A：在当前行尾
	o：在当前行之下新开一行
	O：在当前行之上新开一行
	r：替换当前字符
	R：替换当前字符及其后的字符，直至按ESC键