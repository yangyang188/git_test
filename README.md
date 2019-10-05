# git_test
github测试
## git

### 常用命令

```
# 安装
sudo apt-get install git

# 配置用户
git config --global user.email "you@example.com"
git config --global user.name "Your Name"

# 初始化
git init

# 添加文件
git add .

#提交版本
git commit -m '版本号'

# 查看记录
git log
git log --pretty=oneline
git log --graph --pretty=oneline  # 查看冲突
git reflog  # 查看历史记录
git status  # 查看当前工作状态

# 回退版本
git reset --hard HEAD^
git reset --hard HEAD~1
git reset --hard 编号


git checkout -- <文件>...  # 丢弃工作区的改动

git reset HEAD <文件>...  # 以取消暂存

git diff HEAD -- code.txt  # 对比工作区和提交的版本的不同

git diff HEAD^ HEAD -- code.txt  # 对比HEAD和HEAD^ 版本的不同

```

### 分支

```
# 查看分支
git branch

# 切换分支
git checkout -b dev
git checkout master

# 合并分支
git merge dev
git merge --no-ff -m '禁用fast-forward' dev

# 删除分支
git branch -d dev

# 保存未完成的工作区
git stash

# 恢复未完成工作区
git stash list
git stash pop 
```

### github
```
# ssh
ssh-keygen -t rsa -C "xxx@qq.com"

# 克隆
git clone

# 推送远程分支
git push origin <分支名>

# 跟踪远程的分支
git branch --set-upstream-to=origin/<smart> <smart>

# 拉取
git pull origin smart

```

