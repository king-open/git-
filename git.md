# git 本地仓库
**git init** --创建本地仓库.git \
**git add** --哪些文件是需要提交的\
**git ignore** --描述哪些变动不需要提交的\
**git commit -m** --意思是请把当前代码复制一次到.git目录，字符串意思是提交的理由\
**git commit -v** --能帮忙回顾刚刚改了什么，迫使把提交的理由写的清楚一些

---
### 已经创建拷贝 - 可以通过 **git log** 查看\
## 修改后再次提交
**git add**\
**git commit -v** 重复两个操作即可\
**git commit --hard xxxxx**  用来切换版本。\xxx是提交号的前六位(用git log) 确保已经把所有代commit \ 因为这个操作会使没有commit 过的变动消失

----
### 分支

**git branch** --基于当前commit创建一个新的时间线\(分支)
**git checkout** --用于切换另一个分支 当前目录有未\提交的代码，只要跟另一个分支不冲突，就不需要理会

----
### 分支合并 -git merge x 
合并时会有conflict 提示\
使用 **git status** 查看哪个文件冲突打开文件搜索====(四个等号)在上下两部分中选择要保留的代码 删除\====>>><<<这些标记

**git add** 对应文件
再次**git status**解决下一个文件的冲突直到没有冲突，\运行**git commit** (注意不需要选项)

