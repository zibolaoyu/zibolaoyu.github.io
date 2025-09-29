---
title: 在snap中调用mediapipe手部检测的案例（5）
date: 2025-01-18 11:26:55
tags:
---
首先通过添加库，添加手部检测的库。
![如图1所示](./image/mediapipe/21.png)
手部识别的例子，是‌使用MediaPipe‌的手部部关键点坐标，根据这个坐标值把对应的21个关键点用小红点标注出来，用这些点显示出一只完整手的关键点。然后取食指指尖和拇指指尖两个关键点的x坐标和y坐标的插值，如果插值小于20，则点亮microbit的指示灯。
通过这个例子可以开发一些针对人手交互的例子。代码如下：
![如图2所示](./image/mediapipe/22.png)
本例还通过snap的microblock库和控制microbit实现对硬件灯的控制。相关代码如下图：
![如图3所示](./image/mediapipe/23.png)
在microblock中对microbit设置相关代码如下图所示：
![如图4所示](./image/mediapipe/24.png)

演示案例: 
[example-5](https://snap.codelab.club/snap.html#open:https://zibolaoyu.github.io/post/mediapipe/hand.xml)