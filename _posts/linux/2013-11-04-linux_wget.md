---
layout: linux
title: "linux_wget 下载"
description: "linux wget下载"
category: "linux"
tags: [wget,linux]
---
{% include JB/setup %}


 4 建立简单的robots.txt文件：

$ cat robots.txt
User-agent: *
Disallow: rocrocket-2.html

    这个文件的内容就是要屏蔽rocrocket-2文件的下载和spider。

    5 我们用wget来下载这个测试站点：

wget -r http://my-test.cn:61212/

$ ls -1
index.html
robots.txt
rocrocket-1-1.html
rocrocket-1-2.html
rocrocket-1.html

    看！下载到的包含了robots.txt文件，但没有包含rocrocket-2及其相关的文件。

    可见，robots.txt生效了，wget遵守了robots.txt的规则！

    6 我如何突破robots.txt的限制呢？

    使用-execute选项就可以，这个选项的作用是将其后的参数模拟“放到.wgetrc中的执行效果”。

$ wget -r --execute robots=off http://jx-nsop-test0.jx:61212/

$ ls -1
index.html
rocrocket-1-1.html
rocrocket-1-2.html
rocrocket-1.html
rocrocket-2-1.html
rocrocket-2-2.html
rocrocket-2.html
