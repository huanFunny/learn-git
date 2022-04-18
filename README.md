# learn-git

> A Vue.js project

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

## Git

``` bash
# git 安装

# 检测是否安装git
git --version

#从远程git仓库复制项目
git clone <git_url>

# git 初始化
git init

# 配置git仓库地址
git remote add [name] [git_url]
# 修改git仓库地址
git remote set-url [name] [git_url]
# 删除源地址
git remote remove [name]

# 提交工作区所有文件到暂存区
git add .
# 将暂存区中的文件提交到本地仓库中，即打上新版本
git commit -m 'message'
# 同步远程仓库
git pull origin [分支]
# 向远程分支上推送内容
git push origin master

# 显示本地仓库的所有分支
git branch
# 创建分支
git branch <branch_name>
# 切换分支
git checkout <branch_name>
# 创建并切换分支
git checkout -b <branch_name>
# 将当前分支与指定分支进行合并
git merge <branch_name>
#删除分支
git branch -d <branch_name>

# 配置个人的用户名称和电子邮件地址
git config --global user.name "wyh"
git config --global user.email wyhdml608@126.com
```
