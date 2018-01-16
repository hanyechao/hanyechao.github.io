---
layout: post
title: "ant design环境部署"
date: 2018-01-16 21:33
description: "ant design环境部署"
tag: 测试框架
---  

## ant design环境部署
### ant design官方配置说明
[http://design.alipay.com/develop/web/react/getting-started](http://design.alipay.com/develop/web/react/getting-started)

### node.js教程
[http://www.runoob.com/nodejs/nodejs-tutorial.html](http://www.runoob.com/nodejs/nodejs-tutorial.html)

### es6学习教程
[http://es6.ruanyifeng.com](http://es6.ruanyifeng.com)

### mac环境
1. 配置[node.js](http://nodejs.cn/download/)环境
2. 终端输入安装脚手架命令：npm install antd-init -g </br>
说明：由于npm服务器在国外，所以国内访问下载依赖速度比较慢，时常下载超时或者失败，所以淘宝提供一套国内下载依赖的命令，就是cnpm，cnpm与npm使用命令一致，只需要把npm替换成cnpm
3. 【2】安装完后，执行操作：mkdir antd-demo && cd antd-demo
4. 输入antd-init，初始化ant项目内容

### 遇到的坑
1. node xxx.js 或者 npm start 运行js服务时候，强行终止服务而非npm stop正常停止，下次再次启动时候，可能会出现启动异常，可以确认是端口冲突引起的，ps -ef | grep “node” 查询进程服务的pid，kill掉，再执行启动服务就可以了