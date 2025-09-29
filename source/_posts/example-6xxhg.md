---
title: 在snap中实现一元线性回归（进行图书价格预测）
date: 2025-01-21 11:26:55
tags:
---
首先收集一些图书价格和图书页数的数据，如表所示。
![如图1所示](./image/jqxx/1.png)
从这些数据出发建立模型，找出图书价格与图书页数的关系，然后，如果我们有一本书知道其页数，根据得出的关系就可以预测出这本书的价格。
这个例子我们用到一个scisnap!v3的库如图所示：
![如图2所示](./image/jqxx/2.png)
要运行scisnap!v3,需要用到JavaScript扩展，要在设置中勾选该项，相关设置如图：
![如图3所示](./image/jqxx/3.png)
将表中的数据绘制成散点图，其中横轴表示图书页数，纵轴表示图书价格，
![如图4所示](./image/jqxx/4.png)
从图中可以看出，这些点大致分布在一条直线附近，因此称这两个量之间具有线性关系，这条直线也被称之为回归直线，如下图所示：
![如图5所示](./image/jqxx/5.png)
如果能求出这条直线的方程，就可以了解图书价格与图书页数的大致关系，也就可以根据页数大致预测图书价格

演示案例: 
[example-6](https://snap.codelab.club/snap.html#open:https://zibolaoyu.github.io/post/jqxx/tushujiageyuce.xml)