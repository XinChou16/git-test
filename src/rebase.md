
[refer](https://learngitbranching.js.org/?nodemo)

## Scene

1. 本地分支落后新的分支
2. 远程分支和本地分支都修改了同一个文件

## Solution

使当前的更改基于远程最新分支

方法一：
1. `git fetch`
2. `git rebase origin/master`
3. `git push`

方法二：

```shell
git fetch
git merge origin/master
git push
```

等同于 
`git pull; git push`

注：
- `git pull` 为 `git fetch` 和 `git merge` 简写
- `git pull --rebase` 为 `git fetch` 和 `git rebase` 的简写


简化版本

核心命令
```shell
git pull --rebase
git push
```

遇到冲突：
1. 解决冲突
2. 解决完 git add 添加该文件
3. git rebase --continue
4. 推送到远端

```shell
git add README.md
git commit
git pull --rebase
git add README.md 解决冲突
git rebase --continue
git push
```





