## git指令
到本地
- 提交
```asm
git add 文件名

```
- 上传
```asm
git commit -m "评论"
```
- git pull
```asm
git pull 命令用于从远程获取代码并合并本地的版本
相当于git fetch 和 git merge
一般推荐用git fetch
```
- git log 查看提交日志
- git status 查看当前状态

## 工程 git
- Branch 切分支
```asm
git checkout 切换到已有分支
git checkout -b 切换到新分支
```
- 合并冲突
    1. 要把yin分支的一个新特性(功能)合并到master分支上
    2. 但是两个分支都有修改，并且修改共同的文件，共同的位置(都是第四行).
```asm

```