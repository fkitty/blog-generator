---
title: Hexo的使用
date: 2017-12-09 15:56:54
tags:
---
1.进入桌面 cd ~/Desktop
2.在GitHub上建一个空仓库，仓库名称是tuoanqi.github.io
3.安装Hexo  npm install -g hexo-cli
4.hexo init myBlog
5.cd myBlog
6.npm i
7.hexo new myfirsthexo(会显示一个路径)
8.start  (这里的路径中的斜杠要反过来),编辑博客内容
9.start _config.yml,编辑网站配置
   第六行的title改为使用Hexo+GitHub搭建博客
   第九行的author改为tuoanqi
   把最后一行的type改成type: git(注意空格)
   在最后一行后面新增一行，左边与type平齐，加上一行repo: 仓库地址(注意repo后面也有空格，地址使用ssh地址)
10.npm install hexo-deployer-git --save,安装git部署插件
11.hexo deploy
12.进入GitHub的GitHub pages功能中，选择master branch
   然后h会生成一个预览连接，就可以查看了。


！！！再创建一个博客
cd myBlog要在这个目录下
1.hexo new 使用Hexo+GitHub搭建自己的博客
2.start 第一步生成的路径
3.hexo generate
4.hexo deploy
5.查看即可


