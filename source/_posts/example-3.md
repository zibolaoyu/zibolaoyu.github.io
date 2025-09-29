---
title: 在snap中调用mediapipe的案例
date: 2025-01-16 11:26:55
tags:
---
‌MediaPipe‌是由Google Research开发的一款开源框架，旨在帮助开发者轻松地构建、测试和部署复杂的多模态、多任务的机器学习模型，特别擅长于实时处理和分析音频、视频等多媒体数据‌
应用场景和示例
1‌姿态估计‌：MediaPipe可以实时检测和追踪人体的关键点（如肩膀、肘部、膝盖等），并估计人体的姿态，适用于体育训练、动作捕捉、增强现实等应用‌。
2‌手部追踪‌：能够检测和追踪手部的关键点，提供手势识别和手部动作分析的能力，适用于手势控制、虚拟现实、手写输入等应用‌。
3‌人脸检测‌：用于识别图像或视频中的人脸，适用于安全监控、人脸识别登录等场景‌。
4‌物体检测‌：可以识别和检测图像或视频中的物体，适用于各种视觉相关的应用‌。
5‌运动追踪‌：提供运动追踪功能，适用于需要分析人体或动物运动的应用‌。

mediapipe 提供了 JavaScript API, 可以通过 JavaScript function 将 mediapipe 引入到 Snap! 中。
import() 可以将 ECMAScript 模块异步动态加载到非模块环境中。
在[https://snap.codelab.club/](https://snap.codelab.club/)可以导入 ,相关的mediapipe 库（人脸检测、手部检测、姿态检测）。在snap中使用mediapipe库，不需要修改底层代码，只需要用拖拽程序块的方式，就能体验，非常适合中小学生使用。早期尝试过在anaconda终使用mediapipe进行教学，后来又把他移植到xedu环境终，发现学生学习效果都不能达到自己要求，所以在snap中尝试一下。
种瓜提供的
[国内体验案例](https://snap.codelab.club/snap.html#open:https://wwj718.github.io/post/img/mediapipe-Gesture-Recognition-cn.xml&enableJS)