---
layout: post
title: "git保存密码的方法"
category : 
tags : []
group: navigation
---


##windows7 配置如下：

*创建_netrc文件，内容为

>machine your.server.com

>login your-username

>password your-password

*创建run.bat，内容为：

>setx HOME %USERPROFILE%

>copy _netrc %USERPROFILE%

>pause

*两个文件放到同一目录下，执行run.bat即可。