# gitbook使用简介

使用gitbook结合github提供的pages功能，可以让你非常方便的搭建起自己的知识管理平台，你可以把你日常的读书笔记、工作总结、方法论、以及任何有被记录价值的信息，记录在上面。然后，你可以随时随地通过网页来访问这些内容；

## 01 本地编辑md文档

在本地通过typora新建md文档，并在SUMMARY.md文件下指定文件目录；

## 02 构建部署发布

在cmd窗口下执行命令：

gitbook build

gitbook serve

## 03 浏览器访问本地

发布后，在本地浏览器访问：http://127.0.0.1:4000，即可访问添加的文档

## 04 上传项目到github

1) 右键单击桌面空白处，选择Git Bash Here，进入git控制台

2)将github项目clone到本地（用于保存gitbook编译生成的静态网页文件），执行命令：

git clone 项目地址

3）将gitbook编译生成的静态网页文件复制到git本地项目文件夹

4）上传本地静态网页项目到github，执行命令：

首次上传项目：

git add ./*

git commit -m 'update'

git push 

编辑修改项目内容：

git rm -r --cache ./*

git add .

git commit -m "git ignore before"

## 05 配置github项目的github pages

![](https://wangzaolin.github.io/SoftwareTest/mybook/img/githubPages.png)

## 06 浏览器访问线上文档

在浏览器访问：https://wangzaolin.github.io/Software/  (https://github账号.github.io/项目名称)，即可访问添加的文档；

