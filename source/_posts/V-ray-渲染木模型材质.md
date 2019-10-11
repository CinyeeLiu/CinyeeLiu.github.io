---
title: V-ray 渲染木模型材质
date: 2019-10-10 23:30:11
tags: 
cover: https://blog-1300344724.cos.ap-chengdu.myqcloud.com/img/vary_for_su_model1.png
---
# V-ray 渲染激光切割木模型
在出表现图的时候经常会遇到需要贴模型照片，但是模型在交图之前可能还没有。所以为了投机取巧，
* 可以第二天贴模型照片，这样的效果更好，但是图面整体性不好
* 用v-ray附上木头材质渲染出模型效果

这里主要讲第二种方法。

## 准备工作
软件：`sketchup 2019` `V-ary for su 4.0`
* 首先得有一个打板用的模型，全部炸开选中为默认图层，删除其他所有图层
* 新建两个图层：**正面** 和 **侧面**，因为木板材激光切割打出来侧面是烧焦的黑色
* 一个个的选中你模型的侧面放在侧面图层，选中剩下的放在正面图层
* 接下来就是选择合适的材质以及调节参数
* 打开vray,调出vray资源管理器
* 在左边材质-`wood & laminate`里找到`laminate A02 120cm`这个材质,拖入资源管理器 ![](https://blog-1300344724.cos.ap-chengdu.myqcloud.com/img/Snipaste_2019-10-12_00-18-39.png)
* 打开`laminate A02 120cm`这个材质在`通用`-`VRayBRDF`-`漫反射`里面找到一个**田**字的图案（叫纹理插槽）![](https://blog-1300344724.cos.ap-chengdu.myqcloud.com/img/Snipaste_2019-10-12_00-23-50.png)
* 右键`套嵌`-`颜色校正`（老版本也可以剪切）![](https://blog-1300344724.cos.ap-chengdu.myqcloud.com/img/Snipaste_2019-10-12_00-24-37.png)
* 在`颜色校正`里面调节`颜色/输入` `亮度` `对比度`**等等**参数，正面亮度较高，侧面烧焦的亮度低。![](https://blog-1300344724.cos.ap-chengdu.myqcloud.com/img/Snipaste_2019-10-12_00-29-19.png)
* 回到材质最开始的界面,调节`漫反射`，和`反射`里面的`反射光泽度`，烧焦的侧面光泽度稍微高一些，正面和侧面反射都很低![](https://blog-1300344724.cos.ap-chengdu.myqcloud.com/img/Snipaste_2019-10-12_00-29-32.png)
* 复制这个调好的材质，然后调节第二个面（正面或者侧面）其他各种参数调节可以慢慢试，我只试了这些。
* 下面是效果图
![](https://blog-1300344724.cos.ap-chengdu.myqcloud.com/img/vary_for_su_model1.png)
![](https://blog-1300344724.cos.ap-chengdu.myqcloud.com/img/4.png)
![](https://blog-1300344724.cos.ap-chengdu.myqcloud.com/img/2.png)

