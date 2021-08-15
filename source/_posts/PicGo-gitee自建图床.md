---
title: PicGo+gitee自建图床
tags: 
  - 教程
  - 分享
abbrlink: 8ef9b6b2
date: 2021-08-16 01:13:28
---

# PicGo+gitee自建图床

## 前言

​	大前天因为我的不当操作被迫重置电脑，结果电脑上好多东西没了，这两天陆陆续续把一些日常使用的环境，软件啥的都配置好了，结果今天水贴的时候发现PicGo用不了了，刚好借此机会分享一波

## 优点

* 方便快捷，如果使用typora写作，直接粘贴图片即可
* 速度快，体验有保证：gitee是国内网站，速度没得说
* 成本低：几乎零成本

## 缺点

gitee限制只能上传1M以内的图片，超过1M不显示

但也可以通过PicGo内的compress插件解决这个问题

## 下载PicGo

github上免费下载：[下载地址](https://github.com/Molunerfinn/PicGo/releases/tag/v2.3.0-beta.6)

## 安装Node.js

[下载地址](https://nodejs.org/en/)

选14就可以

安装好后记得win+r 输入cmd 然后回车打开命令提示符

然后输入`node -v`出现版本号后就没问题，如图

![image-20210801155456634](https://gitee.com/augustusxue/augustu_image/raw/master/img/20210801163608.png)

安装好后记得重启电脑

## 安装gitee插件

![image-20210801155529380](https://gitee.com/augustusxue/augustu_image/raw/master/img/20210801163605.png)

插件设置->输入`gitee`->随便选择一个，我选了第一个->安装

如果安装过程时间太长，可以在cmd窗口里输入这条命令，改用淘宝源

`npm config set registry https://registry.npm.taobao.org`

## gitee设置

登录gitee.com（没有的话需注册）

![image-20210801160017553](https://gitee.com/augustusxue/augustu_image/raw/master/img/20210801163602.png)

右上角新建仓库，推荐叫***_image

找了张图，大概这样子

![](https://pic4.zhimg.com/v2-11790828fe9ce436ea6d92fbe1c0662f_b.jpg)

创建好后创建个人令牌

![image-20210801160517445](https://gitee.com/augustusxue/augustu_image/raw/master/img/20210801163554.png)

右上角个人头像->设置->左半边下拉->私人令牌

![image-20210801160608957](https://gitee.com/augustusxue/augustu_image/raw/master/img/20210801163551.png)

![image-20210801160629518](https://gitee.com/augustusxue/augustu_image/raw/master/img/20210801163548.png)

获得token后复制到记事本上待用

## picgo插件设置

左半栏->图床设置->gitee图床

![image-20210801161041159](https://gitee.com/augustusxue/augustu_image/raw/master/img/20210801163545.png)

打开gitee->进入仓库->查看网页链接

比如我的链接是https://gitee.com/augustus***/augustu_image

那么我的

owner就填写augustus***

repo就填写augustu_image

path如果不填的话就默认存放根路径，我创建了一个img文件夹，填写img，图片就会存放进img里

token:刚刚我们复制的私人令牌

message:你写啥都行，不写也可以

然后点击确定，点击设置为默认图床，OK！

## 使用

![image-20210801162151678](https://gitee.com/augustusxue/augustu_image/raw/master/img/20210801163542.png)

直接拖入框中即可，链接会自动粘贴到剪贴板，还可以通过相册回看

## Typora配置



![image-20210801163701199](https://gitee.com/augustusxue/augustu_image/raw/master/img/20210801163701.png)

插入图片时选择自动上传图片

PicGo路径选择自己的PicGO安装的地方

最后验证图片上传选项，出现success的话就是成功
