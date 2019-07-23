---
description: >-
  Flutter 是 Google推出并开源的移动应用开发框架，主打跨平台、高保真、高性能。开发者可以通过 Dart语言开发 App，一套代码同时运行在
  iOS 和 Android平台。
---

# Flutter 简介

## **跨平台**

Flutter 与其他框架不同，Flutter 不使用WebView，也不使用平台系统的任何原生控件。 相反，Flutter使用自己的高性能渲染引擎来绘制和渲染页面。这样不仅可以保证在Android和iOS上UI的一致性，而且也可以避免对原生控件依赖而带来的限制及高昂的维护成本。

Flutter 底层使用Skia作为其2D渲染引擎，Skia是Google的一个2D图形处理函数库，包含字型、坐标转换，以及点阵图都有高效能且简洁的表现，Skia是跨平台的，并提供了非常友好的API，目前Google Chrome浏览器和Android均采用Skia作为其绘图引擎，值得一提的是，由于Android系统已经内置了Skia，所以Flutter在打包APK\(Android应用安装包\)时，不需要再将Skia打入APK中，但iOS系统并未内置Skia，所以构建iPA时，也必须将Skia一起打包，这也是为什么Flutter APP的Android安装包比iOS安装包小的主要原因。高效率

## 高性能

Flutter App 之所以高性能主要是取决于一下2点 ：

* 采用 Dart 语言开发。在 Flutter 开发中，Dart 支持 JIT \(即时编译\)，可以提高开发效率，但是再 App 发布的时候，Dart 支持将您的代码编译成机器码，这时候您的Dart代码效率将会达到最高，当以 AOT模式运行时，速度的提升对高帧率下的视图数据计算很有帮助。
* Flutter使用自己的渲染引擎来绘制UI，编译了类似 React Native 需要JSBridge中间的消耗，并且直接对接绘制系统，减少系统框架层次调用，使您的 App 性能达到最佳

## 高效率开发

Dart 支持 JIT 和 AOT 模式运行：

**基于JIT的快速开发周期**：Flutter在开发阶段采用，采用JIT模式，这样就避免了每次改动都要进行编译，极大的节省了开发时间，并且刷新时间在毫米界别。

**基于AOT的发布包**: Flutter在发布时可以通过AOT生成高效的ARM代码以保证应用性能。

## 发布时间线：

* 2017 年 Google I/O 大会上，Google 首次推出了一款新的用于创建跨平台、高性能的移动应用框架—— Flutter。
* 2018 年 2 月，Flutter 发布了第一个 Beta 版本，同年五月， 在2018年 Google I/O 大会上，Flutter 更新到了 beta 3 版本。
* 2018年6月，Flutter 发布了首个预览版本，这意味着 Flutter 进入了正式版（1.0）发布前的最后阶段。
* 截止2019 年 7 月， Flutter 发布了 1.7 版本，预示着 Flutter 进入了告诉的发展期

经历了短短2年多的时间，Flutter 生态系统得以快速增长，得到社区的支持，并且取得了开发者的信赖，其未来发展值得期待！  






### 

