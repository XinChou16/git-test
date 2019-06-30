
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



简化版本

```shell
git pull --rebase
git push
```

- `git pull` 为 `git fetch` 和 `git merge` 简写
- `git pull --rebase` 为 `git fetch` 和 `git rebase` 的简写




