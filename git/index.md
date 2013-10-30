---
layout : git
---
#git help
### git 返回上一个版本
	git reset --hard HEAD 

	git reset --hard HEAD^

	git reset --soft HEAD^

###git 放弃最新修改的内容.
	git throwh    //只是一个别名

### 当要修改一些不属于本版本时的一些小修改，但现在此版本又已经进行了改动
	git stash        //隐藏当前的修改
### 在这里可以做出对应的修改再提交
	git stash apply  //把隐藏的取出来回到当前的修改.

###删除分支
	git branch -D 分支号 
###创建fasdfdf版本号的分支
	git checkout fasdfdf -b 分支号
