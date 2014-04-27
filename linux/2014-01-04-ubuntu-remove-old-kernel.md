---
layout: default
title: "ubuntu remove old kernel"
description: ""
category: ""
tags: []
---
{% include JB/setup %}


### ubuntu 删除旧的内核

	sudo aptitude purge ~ilinux-image-.*\(\!`uname -r`\)

** 注 ** 本命令要在bash下面运行才可以
