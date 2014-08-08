---
- layout: default
- title: "ubuntu remove old kernel"
- description: "当ubuntu系统更新后往往会把内核也会更新，这时会产生旧的内核，默认系统不会把旧的内核删除，这时我们就需要手动的把不使用的内核删除"
- category: "ubuntu linux内核"
- tags: []
---
{% include JB/setup %}


### ubuntu 删除旧的内核

	sudo aptitude purge ~ilinux-image-.*\(\!`uname -r`\)

** 注 ** 本命令要在bash下面运行才可以运行。
