---
layout: post
title: 如何新建一个vue项目
data: 2019-06-06
author: "zzw"
header-img: "../img/20190606/2019-06-06.jpg"
catalog: true
tags:
    - vue
---


## 新建vue项目的具体步骤

1.首先安装node

进入[官网](https://nodejs.org/en/download/current/)下载与电脑相匹配的版本，安装完成后，打开命令行输入` node -v `,出现版本信息表示安装成功。npm包管理器，是集成在node中的，所以，直接输入 ` npm -v `就会如下图所示，显示出npm的版本信息。

![img](/img/20190606/node-v.png)

2.由于有些npm有些资源被屏蔽或者是国外资源的原因，经常会导致用npm安装依赖包的时候失败，所以还需要npm的国内镜像---cnpm。在命令行输入` npm install -g cnpm registry=http://registry.npm.taobao.org `.

3.安装vue-cli，命令行输入` cnpm install -g vue-cli `.

4.安装webpack,` cnpm install webpack-g `

5.选择路径，cd目录路径，新建项目，命令行输入` vue init webpack 项目名称 `,完成项目的相关配置，一般默认都选yes。完成后进入文件夹，可以看到项目结构如下：

![img](/img/20190606/initialize.jpg)

6.启动项目，下载依赖。进入项目目录，命令行下输入` cnpm install `,和` npm run dev `,项目启动成功后，可以在浏览器输入网址 http: //localhost:8080, 如下图所示：

![img](/img/20190606/run.png)
![img](/img/20190606/browser.jpg)


## 实现我们自己的页面

1.先看main.js 项目入口文件

![img](/img/20190606/mainjs.png)

首先导入了vue、vue-router和app.vue，axios是我后来需要引入的。初始化一个vue对象，将router和组件注册到vue对象中。这个文件我们先不用管，不影响我们后面的开发。

2.然后看主容器app.vue

![img](/img/20190606/appvue.png)

App.vue是主组件，所有页面都是在App.vue下进行切换的。组件分为三个部分template、script和style。在单页面应用中，每一个页面对应一个路由，切换路由即可切换页面。

3.看router文件夹下面的index.js

![img](/img/20190606/indexjs.png)

这里我导入了cart和address组件，生成router对象，router对象里可以有很多个路由，每个路由包含了三个字段path,name,component.换成自己的组件，页面就会变成我们自己的页面。需要更详细的构建vue单页应用的过程，可见[参考](https://blog.csdn.net/zgh0711/article/details/78042677)

## 新建vue项目中遇到的各种error

1.启动时报错"Unexpected tab character"

解决方法：在eslint的配置文件中（.eslintrc）rules项中添加一行："no-tabs":"off"；或者在报错的文件前加上：/* eslint-disable */

2.启动时报错"Mixed spaces and tabs"

解决办法：由于使用了Eslint来规范代码，如果不想受限严格可以在报错的文件前加上：/* eslint-disable */

