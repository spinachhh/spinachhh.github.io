

15:39:48
故渊 2019/6/9 15:39:48
https://segmentfault.com/a/1190000009871504
17:15:37
故渊 2019/6/9 17:15:37

17:52:53
池鱼 2019/6/9 17:52:53
---
layout: post
title: 如何新建一个vue项目
data: 2019-06-06
author: "zzw"
header-img: ""
catalog: true
tags:
    - vue
---


## 新建vue项目的具体步骤

1.首先安装node

进入[官网](https://nodejs.org/en/download/current/)下载与电脑相匹配的版本，安装完成后，打开命令行输入` node -v `,出现版本信息表示安装成功。npm包管理器，是集成在node中的，所以，直接输入 ` npm -v `就会如下图所示，显示出npm的版本信息。

![img](../img/20190606/node-v.png)

2.由于有些npm有些资源被屏蔽或者是国外资源的原因，经常会导致用npm安装依赖包的时候失败，所以还需要npm的国内镜像---cnpm。在命令行输入` npm install -g cnpm registry=http://registry.npm.taobao.org `.

3.安装vue-cli，命令行输入` cnpm install -g vue-cli `.

4.安装webpack,` cnpm install webpack-g `

5.选择路径，cd目录路径，新建项目，命令行输入` vue init webpack 项目名称 `,完成项目的相关配置，一般默认都选yes。完成后进入文件夹，可以看到项目结构如下：

![img](../img/20190606/initialize.png)

6.启动项目，下载依赖。进入项目目录，命令行下输入` cnpm install `,和` npm run dev `,项目启动成功后，可以在浏览器输入网址

18:23:02
池鱼 2019/6/9 18:23:02

18:43:13
故渊 2019/6/9 18:43:13

22:13:08
故渊 2019/6/9 22:13:08


对方已成功接收了您发送的离线文件“browser.jpg”(38.12KB)。
23:14:57
池鱼 2019/6/9 23:14:57

23:17:08
池鱼 2019/6/9 23:17:08
2019-06-06
23:22:02
故渊 2019/6/9 23:22:02


故渊 2019/6/9 23:23:45

23:24:57
对方已成功接收了您发送的离线文件“2019-06-06.jpg”(61.60KB)。
23:34:53
池鱼 2019/6/9 23:34:53
---
layout: post
title: 如何新建一个vue项目
data: 2019-06-06
author: "zzw"
header-img: ""
catalog: true
tags:
    - vue
---


## 新建vue项目的具体步骤

1.首先安装node

进入[官网](https://nodejs.org/en/download/current/)下载与电脑相匹配的版本，安装完成后，打开命令行输入` node -v `,出现版本信息表示安装成功。npm包管理器，是集成在node中的，所以，直接输入 ` npm -v `就会如下图所示，显示出npm的版本信息。

![img](../img/20190606/node-v.png)

2.由于有些npm有些资源被屏蔽或者是国外资源的原因，经常会导致用npm安装依赖包的时候失败，所以还需要npm的国内镜像---cnpm。在命令行输入` npm install -g cnpm registry=http://registry.npm.taobao.org `.

3.安装vue-cli，命令行输入` cnpm install -g vue-cli `.

4.安装webpack,` cnpm install webpack-g `

5.选择路径，cd目录路径，新建项目，命令行输入` vue init webpack 项目名称 `,完成项目的相关配置，一般默认都选yes。完成后进入文件夹，可以看到项目结构如下：

![img](../img/20190606/initialize.jpg)

6.启动项目，下载依赖。进入项目目录，命令行下输入` cnpm install `,和` npm run dev `,项目启动成功后，可以在浏览器输入网址 http://localhost:8080,如下图所示：

![img](../img/20190606/run.png)
![img](../img/20190606/browser.jpg)


## 实现我们自己的页面

1. 先看main.js 项目入口文件

![img](../img/20190606/mainjs.png)

2.然后看app.vue

![img](../img/20190606/appvue.png)

## 新建vue项目中遇到的各种error

池鱼 2019/6/9 23:35:52
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

![img](../img/20190606/node-v.png)

2.由于有些npm有些资源被屏蔽或者是国外资源的原因，经常会导致用npm安装依赖包的时候失败，所以还需要npm的国内镜像---cnpm。在命令行输入` npm install -g cnpm registry=http://registry.npm.taobao.org `.

3.安装vue-cli，命令行输入` cnpm install -g vue-cli `.

4.安装webpack,` cnpm install webpack-g `

5.选择路径，cd目录路径，新建项目，命令行输入` vue init webpack 项目名称 `,完成项目的相关配置，一般默认都选yes。完成后进入文件夹，可以看到项目结构如下：

![img](../img/20190606/initialize.jpg)

6.启动项目，下载依赖。进入项目目录，命令行下输入` cnpm install `,和` npm run dev `,项目启动成功后，可以在浏览器输入网址 http://localhost:8080,如下图所示：

![img](../img/20190606/run.png)
![img](../img/20190606/browser.jpg)


## 实现我们自己的页面

1. 先看main.js 项目入口文件

![img](../img/20190606/mainjs.png)

2.然后看app.vue

![img](../img/20190606/appvue.png)

## 新建vue项目中遇到的各种error
