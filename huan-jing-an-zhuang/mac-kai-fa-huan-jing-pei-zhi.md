---
description: 本文将介绍如何在 Mac OS 下配置 Flutter 开发环境
---

# Mac OS 开发环境配置

{% hint style="info" %}
Mac OS 可以同时编译 Android App 与 iOS App
{% endhint %}

## 开发环境配置

### 设置中国镜像

```bash
 export PUB_HOSTED_URL=https://pub.flutter-io.cn
 export FLUTTER_STORAGE_BASE_URL=https://storage.flutter-io.cn
```

### 下载 Flutter SDK 

#### Git 方式：

```bash
git clone -b dev https://github.com/flutter/flutter.git
```

#### 下载 SDK 包

访问：[https://flutter.dev/docs/development/tools/sdk/releases?tab=macos](https://flutter.dev/docs/development/tools/sdk/releases?tab=macos) 下载您需要的 SDK 版本

### 运行环境检查

```bash
export PATH="$PWD/flutter/bin:$PATH"
$ cd ./flutter
$ flutter doctor
```

如果其中出现错误，只需要根据提示解决问题即可

