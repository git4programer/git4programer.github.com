---
layout: vim
title: "vim的复制与粘贴"
description: "vim复制，vim粘贴"
category: "vim"
tags: []
time : 20/10/2013 23:31:04
---

##vim的复制与粘贴问题。

vim是文本编辑器，既然是文本编辑器，那么就会要用到复制与粘贴的功能。

vim中一般复制是用yy，粘贴用的是p或者大P，其中yy表示复制当前光标的所在行，
如果想复制多行，则可以在yy的前面加上数字：如我想复制当前光标以下的10行，
则只要按10yy就可以把内容复制到粘贴板了。而粘贴小p与大P的区别是粘贴在当前行下
与当前行上的区别。

vim的复制还有别一种办法，那就是选中(v 进入可视行，ctrl+v进入可视块,hjkl移动选择)
复制的字或者是行，选中后再按y.

vim中的剪切命令就是dd 要多行的操作跟yy复制相同，（如剪切当前光标以下10行，10dd）

vim一般的复制粘贴就是这样了，但这些命令并不能把内容复制到系统共享的粘贴板上，
也不能把系统粘贴板上面的内容粘贴到vim当中。

要是你以为vim没有这个功能，那你就错啦！

其实vim会把复制到的内容放到十几个寄存器当中，其中有一个就是和系统的粘贴板共享的，
只要我样把内容复制到这个寄存器当中，和把这个寄存器中的内容粘贴到vim上那问题就可以
解决了。

这个寄存器的名字就是＋，

那如何把内容复制到寄存器当中呢？

那就是在复制之前按\"加上寄存器的名 再加上 y 就可以了
同样要把寄存器中的内容粘贴到vim当中，只要在粘贴前先按" 加上寄存器的名 再加上小p或者大P
就可以了。

那么vim的寄存器有十多个，怎么知道寄存器放的复制内容是什么呢？

进入命令行模式，reg就可以查看每一个寄存器中的内容了。
其中最后一次复制或者删除的就放在第一个寄存器当中，再次复制或者删除又会把它放在第一个寄存器
当中，原来在这个寄存器中的内容就会放到下一个中，最后就会把第十个寄存器当中的内容丢掉。