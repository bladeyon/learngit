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

> 切换远程分支：`git checkout [branch-name]` 或 `git switch [branch-name]`，切换到前一个分支：`git checkout -`

> 以当前分支为基础，创建新的分支 **[branch-name]**，创建后停留在当前分支：`git branch [branch-name]`

> 以当前分支为基础，创建新的分支 **[branch-name]**，创建后切换到新分支：`git checkout -b [branch-name]`

> 在新分支完成任务，切换到主分支 `git checkout [master]`，将 **[branch-name]** 合并到 **[master]** 分支 `git merge [branch-name]`；在合并中出现冲突时，手动解决所有冲突，再提交 `git commit -am "解决冲突"`，然后推送 `git push`

> 如果新分支需要 push 到远程分支，则需要切换到 **[branch-name]**，执行 `git push --set-upstream origin [branch-name]`；如果不需要 push，删除即可 `git branch -d [branch-name]`。

> 删除远程分支 `git push -d origin [branch-name]`

### 练习回退

> 回到某一次提交：`git reset [hash]` （回退后，重置暂存区，保留工作区的修改）、 `git reset --hard [hash]`（回退后，重置暂存区和工作区，即回到 [hash] commit 时的状态）；回到上一次提交：`git reset --hard`，撤销 reset 操作： `git reset --hard [hash]` （hash 为退回之前的 commit 的 hash）。reset 的操作是通过移动 `HEAD（引用指针）` 实现

> 回滚到某次提交：`git revert [hash]` （回滚后是，[hash] 提交前的状态，[hash]及以后的修改以冲突的方式存在工作区），并**生成新的 commit**，这样的好处是每一次提交的历史记录都是完整的；可以执行 `git revert --abort` 撤销本次回滚
