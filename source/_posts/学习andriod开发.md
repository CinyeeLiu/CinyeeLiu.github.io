---
title: 学习andriod开发
date: 2018-10-14 16:39:53
tags: [学习,随笔]
categories: #"技术","学习","Andriod"
    - 技术
    - 学习
    - Andriod
---

# 前言

突然想重拾下代码，决定从andriod开始，在**laocao**的推荐下找到了**第一行代码**这本书。

于是就打印了下来（别问为什么不支持正版）


# 遇到的小困难

安装书中的提示下载了andriod stdio的win版安装包（应该是老版本的2.2几），按照提示安装完成后，创建了第一个经典的project----“hello world”。

AS还自带了手机模拟器，可以直接将写好的程序在模拟器上运行。



可是在编译最初的原始生成的helloworld时，却出现了问题，显示`error:run time out`

因为这段时间也比较忙，我就直接搁置了几天。

参考了一些博客：[Android Studio导入新项目,gradle报 read timed out的情景之一](https://blog.csdn.net/ha_cjy/article/details/79693910)

<escape><!-- more --></escape>

JDK就是Java Development Kit,网上找一个下好，再改下AS的路径就解决了



然后又有新的问题`error: SSL peer shut down incorrectly`

参考:[Error:SSL peer shut down incorrectly的解决方法](https://blog.csdn.net/Ceciiiilia/article/details/69938977)

最后终于运行成功hello world 

![](https://i.imgur.com/hZqwPi4.jpg)
yeah!!!