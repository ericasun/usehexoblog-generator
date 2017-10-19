---
title: 如何使用Hexo搭建博客
date: 2017-10-19 22:26:23
tags:
---
第1步：创建一个目录（建议：别在根目录 ） mkdir hexoblog
第2步：进入目录 cd hexoblog
<<<<<<< HEAD
第3步：在 GitHub 上新建一个空 repo ,repo 名称是「仓库名.github.io」（仓库名一定要这个格式）
=======
第3步：在 GitHub 上新建一个空 repo ,repo 名称是「仓库名.github.io」（一定要是这个格式）
>>>>>>> 8332ab5f0ef319188abb02ce64feb7c2d5e8f14c
第4步：安装Hexo，执行命令 npm install -g hexo-cli
第5步：创建博客系统 hexo init myBlog
第6步：进入博客系统 cd myBlog
第7步：安装模块 npm i
第8步：创建博客（文章） hexo new 开博大吉（开博大吉为文章标题），返回一个 md 文件的路径
第9步：start xxxxxxxxxxxxxxxxxxx.md，编辑这个 md 文件，内容在第二个---之后编写
      （注意：Ubuntu 系统用 xdg-open xxxxxxxxxxxxxxxxxxx.md 命令）
第10步：编辑网站配置 start _config.yml（该文件在hexoblog根目录下）
        可改项：
        1. 第 6 行的 title 文章标题
        2. 第 9 行的 author 作者名
        必改项：
        1. type 改成 type: git
        2. 在最后一行，与 type 垂直对齐，加上一行 repo: 仓库地址（repo: 后面有个空格）
        （仓库地址为firstblog所对应的地址，仓库地址以 git@github.com:）
第11步：安装 git 部署插件 npm install hexo-deployer-git --save
       （之后再修改博客需要上传，可执行：hexo generate代替该步）
第12步：上传博客系统（包括文章）hexo deploy
第13步：进入「仓库名.github.io」对应的 repo，打开 GitHub Pages 功能（setting中），就可以直接点击预览链接
