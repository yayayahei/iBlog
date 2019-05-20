# git pull --merge vs. --rebase
git pull 是组合命令（git fetch, git merge）的简写命令。
git pull 默认选项是--merge，当拉取远程代码后，将远程分支的最近一次snapshot与当前分支的最近一次snapshot与两个分支的最近共同祖先进行三方合并。
还有一种方式合并代码，就是使用选项--rebase，它的原理是将当前分支rebase到远程分支上。当拉取远程代码后,将当前分支的每一次提交做的修改存在临时文件中，，将当前分支设置为远程分支的最后一次提交，将临时文件中的所有修改按顺序应用于当前分支上。
