# git常用命令
### 拉取远程分支
```git
git pull origin [remoteBranch]
```
### 强制覆盖本地代码（与git远程仓库保持一致）
```git
git fetch --all #拉取所有更新，不同步
git reset --hard origin/master #本地代码同步线上最新版本(会覆盖本地所有与远程仓库上同名的文件)
git pull #再更新一次（其实也可以不用，第二步命令做过了其实）
```
单条执行
```git
git fetch --all &&  git reset --hard origin/master && git pull
```
