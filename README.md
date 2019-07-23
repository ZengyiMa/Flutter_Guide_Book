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

采用 Dart 语言开发。Dart支持 AOT，当以 AOT模式运行时，JavaScript便远远追不上了。速度的提升对高帧率下的视图数据计算很有帮助。其次，Flutter使用自己的渲染引擎来绘制UI，布局数据等由Dart语言直接控制，所以在布局过程中不需要像RN那样要在JavaScript和Native之间通信，这在一些滑动和拖动的场景下具有明显优势，因为在滑动和拖动过程往往都会引起布局发生变化，所以JavaScript需要和Native之间不停的同步布局信息，这和在浏览器中要JavaScript频繁操作DOM所带来的问题是相同的，都会带来比较可观的性能开销。。

## 劣势

动态性和 Hotfix 依然遥遥无期。

## 发布时间线：

* 2017 年 Google I/O 大会上，Google 首次推出了一款新的用于创建跨平台、高性能的移动应用框架—— Flutter。
* 2018 年 2 月，Flutter 发布了第一个 Beta 版本，同年五月， 在2018年 Google I/O 大会上，Flutter 更新到了 beta 3 版本。
* 2018年6月，Flutter 发布了首个预览版本，这意味着 Flutter 进入了正式版（1.0）发布前的最后阶段。
* 截止2019 年 7 月， Flutter 发布了 1.7 版本，预示着 Flutter 进入了告诉的发展期

经历了短短2年多的时间，Flutter 生态系统得以快速增长，得到社区的支持，并且取得了开发者的信赖，其未来发展值得期待！  






### 

