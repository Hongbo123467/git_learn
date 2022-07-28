## git指令
- 提交
```
git add 文件名

```
- 上传
```
git commit -m "评论"

```
- git pull
```
git pull 命令用于从远程获取代码并合并本地的版本
相当于git fetch 和 git merge
一般推荐用git fetch
```
- git log 查看提交日志
- git status 查看当前状态

## 工程 git
- Branch 切分支
```
git checkout 切换到已有分支
git checkout -b 切换到新分支
```
- 合并冲突
    1. 要把yin分支的一个新特性(功能)合并到master分支上
    2. 但是两个分支都有修改，并且修改共同的文件，共同的位置(都是第四行).
```
两种方式
       git merge +分支修订号（每次提交）  （合并时要切到主分支）
       -合并之后会增加一个合并节点
       -出现合并冲突，解决冲突后要添加修改后的文件 运行  git merge continue
       -冲突时
            -HEAD：主分支

       git rebase 
       -不会增加额外的合并节点
       -看不到其他分支的流动方式。隐藏了特性的来源分支。看到的特性是一条直线
       -出现合并冲突，解决冲突后要添加修改后的文件 运行  git rebase continue
       -冲突时
            -HEAD：特性分支
```
- 回退
```
git reset
    -mixed 默认 放入暂存区
    -soft 放到动作区
    -hard 不存

git reflog
    可以查看每一个状态的id（包括reset）
    然后使用git reset id 就可以回退到reset前
```
- 暂存
```
git stash save "评论"
git stash list 暂存列表
```
- 将多个提交合并成一个提交
```
git reset -mixed 到第一次提交
再将文件添加后提交一次
```

- PR/MR
```
   在github的pull request模块进行pull request和merge request
```


