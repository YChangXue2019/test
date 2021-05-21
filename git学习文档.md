git status:查看git状态，在工作区，对应的文件显示的是红色，在暂存区对应的文件显示的是绿色

git add 对应的文件：将工作区中对应的文件添加到暂存区，比如：git add index.html  就是将index.html文件添加到暂存区。

git add . :将工作区中的所有文件添加到暂存区

git commit -m "initial project":将暂存区的文件提交到版本区，初始化项目，"initial project" 必须是双引号

git log:文件提交到版本区后，使用该命令查看相关信息

git diff:比较工作去与暂存区的差异

git diff --cached:比较暂存区与版本区的差异

git diff master:比较工作区与版本区的差异

git reset HEAD <file>：暂存区与版本区保持一致，当了两者不一致时，会将版本区中的内容重置到暂存区，覆盖掉暂存区之前的内容，比如：git reset HEAD index.html 就是将版本区中的index.html中的内容重置到暂存区

git checkout <file>:暂存区（暂存区没有就找版本区）覆盖工作区的内容

git rm <file> --cached：删除暂存区的文件

git commit -a -m <msg>:git add .  git commit -m ""

git reset --hard <version>:恢复版本区指定内容到工作区

git reflog:查看引用版本号


git branch:查看分支

git branch dev:创建开发分支

git chechout dev:切换dev分支

git checkout -b dev:创建并切换dev分支

git branch -d dev:删除dev分支


git merge dev：合并分支到master
git log --oneline --graph:展示历史操作图