## 1.初始化本地仓库

```
git init
```

## 2.选择要提交的内容

```
git add xxx
```

## 3.文件描述不提交的内容

```
.gitignore
```

## 4.提交到本地仓库

```
git commit -m "xxx"
git commit -v (推荐使用这行命令，因为可以提交理由可以写的详细易懂，容易让人理解)
```

## 5.显示之前的提交

```
git log
```

## 6.回退到某个版本

```
git reset --hard xxx
```

## 7.查看所有的提交历史

```
git reflog
```

## 8.查看当前状态

```
git status
```

## 9.创建分支

```
git branch xxx
```

## 10.切换分支

```
git checkout xxx
```

## 11.删除分支

```
git branch -d xxx
```

## 12.将另一个分支合并到当前分支

```
git merge xxx (xxx 就是另一个分支的名字)
```

## 13.解决分支冲突：

1. 首先使用 `git status` 查看冲突文件。
2. 打开冲突文件，进行手动修改。
3. 修改保存好之后，使用 `git add xxx` 和 `git commit` 进行提交。
4. 提交之后，删除无用分支 `git branch -d xxx`。

## 14.上传分支:

```
git remote add origin git@xxxxxxx 建立远程连接
git push origin x:x (把左边本地的 x 分支上传到远程 x 的分支)

git checkout x
git push -u origin x (把本地 x 分支上传到远程 origin 分支)
```
