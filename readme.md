Git is a distributed version control system.

Git is free software distributed under the GPL.

Git has a mutale index called stage;

Git tracks changes of files.

Commit github...

create a new branch dev.

Creating a new branch is quick and simple.

again create dev branch;

on issue-001 edit this;

edit a little,a little

完成 issue-001 后回来继续编辑 dev 分支上的此文件。

再测试一遍

修改文件名：git mv readme.txt readme.md

### 2023 年 5 月 5 日 练习分支合并

> 查看本地分支列表：`git branch`

> 查看远程分支：`git branch -r`

> 切换远程分支：`git checkout [branch-name]` 或 `git switch [branch-name]`

> 以当前分支为基础，创建新的分支 **[branch-name]**，创建后停留在当前分支：`git branch [branch-name]`

> 以当前分支为基础，创建新的分支 **[branch-name]**，创建后切换到新分支：`git checkout -b [branch-name]`

> 在新分支完成任务，切换到主分支 `git checkout [master]`，将 **[branch-name]** 合并到 **[master]** 分支 `git merge [branch-name]`；在合并中出现冲突时，手动解决所有冲突，再提交 `git commit -am "解决冲突"`，然后推送 `git push`

> 如果新分支需要 push 到远程分支，则需要切换到 **[branch-name]**，执行 `git push --set-upstream origin [branch-name]`
