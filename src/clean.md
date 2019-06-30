
## `git clean`

> 清除未被 track 的文件 

**慎用**

synopsis

`git clean [-d] [-f] [-i] [-n] [-q] [-e <pattern>] [-x | -X] [--] <path>…​`

- `git clean --dry-run, -n`：显示将会删除的文件
- `git clean --force, -f`：删除所有未被 track 的文件（不会删除.gitignore中的文件夹/文件）
- `git clean -xf`：删除所有未被 track 的文件
- `git clean -df`：删除当前目录下未被 track 的文件
- `git clean -df dirty/`：删除 dirty 目录下未被 track 的文件

