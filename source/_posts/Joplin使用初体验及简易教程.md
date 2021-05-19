---
title: Joplin使用初体验及简易教程
tags:
  - 教程
  - 分享
abbrlink: c2de814d
date: 2021-05-19 21:47:10
---

## 缘由

​	大概一个多月（也许，我记性很差）之前，浏览github的时候看到了它，当时试了一下，因为界面不尽如人意放弃了它。这两天选修课考试，上网找了些资料分享到群里后，闲暇时间想用手机看看，结果发现手机里竟没什么软件可以打开它，十分失望。

​	说起来还挺巧的，tg关注的一个分享软件的频道恰好推荐给我NotesHub，说是使用github保存数据的在线Markdown笔记服务，让我迫不及待地试了试，结果发现还是基于它自己的服务器，还要注册账号，还只能用github,不能用gitee，github的速度大家懂得都懂，所以无奈放弃。本来想试试别的，结果发现没啥好用的，纯纯写作真是不咋地，导入进去效果不行，而且听说作者人品一般，不符合我这种完美主义者的要求。去github上搜索markdown+android，结果出来的结果都不符合我的要求，排第一的看着不错，结果上次更新是五年前，好家伙！然后找md+多平台，找到了Joplin,大略一试，发现真香。

<img src="https://gitee.com/augustusxue/augustu_image/raw/master/img/20210519204843.png" alt="image-20210519204843182" style="zoom:25%;" />

## 简单设置

​	这个感觉没啥好说的，挺好一软件，就这么整呗，其实虽然是开源的，但我感觉完成度已经很高了。我简单的设置了一下。

### 语言

点击：Tools->Options，语言改成中文简体

![image-20210519205105755](https://gitee.com/augustusxue/augustu_image/raw/master/img/20210519205105.png)

### 外部编辑器

Path:框里面选择外部编辑器的位置，找到所属exe就行了，其实不选也可以，本来颜值就不错，但在PC上我还是偏爱Typora

Arguments:-n

### 同步

#### 坚果云WebDav配置 

同步选择还蛮多的，但是国内适合我们用的就那几个，OneDrive虽然也能用，但是那个速度懂得都懂，我还是倾向于WebDav,而我们国内能用好用的也就只有坚果云了，简单介绍一下使用方法

* 1、注册	感觉这个应该不用多说吧？
* 2、在浏览器右上角处点击自己的用户名->账户信息->安全选项

![image-20210519210210443](https://gitee.com/augustusxue/augustu_image/raw/master/img/20210519210210.png)

![image-20210519210444927](https://gitee.com/augustusxue/augustu_image/raw/master/img/20210519210445.png)

向下滑，找到“添加应用”按钮，点击->输入“joplin”->点击“生成密码”->复制密码->点击“完成”

![image-20210519211303545](https://gitee.com/augustusxue/augustu_image/raw/master/img/20210519211303.png)

点击左侧“我的文件”->创建文件夹“joplin”（不能写错）

![image-20210519211226307](https://gitee.com/augustusxue/augustu_image/raw/master/img/20210519211226.png)

#### PC端同步

回到Joplin

* 左侧选项栏里选择“同步”

* 同步目标选择"WebDav"

* WebDAV URL填写

  ```
  https://dav.jianguoyun.com/dav/joplin
  ```

  一定要写/dav/joplin，而不是/dav，血泪经验啊，还好[一个老哥跟我遇到了相同的问题](https://github.com/laurent22/joplin/issues/3714)

  ![image-20210519211522534](https://gitee.com/augustusxue/augustu_image/raw/master/img/20210519211522.png)

* WebDAV 密码 就填写刚刚复制的密码（忘了也没关系，可以再复制一次）

* 单击“检查同步配置”，显示成功！

#### android同步

大同小异

* 左侧选项栏里选择“配置”
* 同步选择“WebDav”,底下与PC端同样填写
* 测试完后记得上方点保存按钮

### 外观

我选择了“北欧（Nord）”主题，感觉还不错

![image-20210519212553915](https://gitee.com/augustusxue/augustu_image/raw/master/img/20210519212554.png)



  <img src="https://gitee.com/augustusxue/augustu_image/raw/master/img/20210519212646.png" alt="image-20210519212646410" style="zoom: 50%;" />

但是PC端编辑器感觉还是没有Typora好用，小短篇在里面写，长篇文章直接外部编辑器就行了，挺好，说实话。

至于安卓端，不会有人真的用手机写文档吧？我感觉安卓端看着好看就完事儿了，偶尔也能编辑一下，毕竟手机打字真是反人类or2

测试了一下是真的爽，电脑上手机上无缝同步（点击同步按钮，我感觉不算很麻烦），手机上终于可以看md了，也可以简单列下清单，写个笔记啥的
