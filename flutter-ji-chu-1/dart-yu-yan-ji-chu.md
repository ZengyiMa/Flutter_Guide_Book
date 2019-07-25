---
description: Dart 是一种易于学习、 易于扩展、并且可以部署到任何地方的应用编程语言
---

# Dart 语言基础

## 基本示例

```dart
// 定义函数
printInteger(int aNumber) {
  print('The number is $aNumber.'); // 输出到控制台
}

// main 函数，入口函数
main() {
  var number = 42; // 什么和初始化变量
  printInteger(number); // 调用函数
}
```

## Dart 关键字



| [abstract](https://dart.dev/guides/language/language-tour#abstract-classes) | [dynamic](https://dart.dev/guides/language/language-tour#important-concepts) | [implements](https://dart.dev/guides/language/language-tour#implicit-interfaces)  | [show](https://dart.dev/guides/language/language-tour#importing-only-part-of-a-library)  |
| :---: | :---: | :---: | :---: |
| [as](https://dart.dev/guides/language/language-tour#type-test-operators)  | [else](https://dart.dev/guides/language/language-tour#if-and-else) | [import](https://dart.dev/guides/language/language-tour#using-libraries)  | [static](https://dart.dev/guides/language/language-tour#class-variables-and-methods)  |
| [assert](https://dart.dev/guides/language/language-tour#assert) | [enum](https://dart.dev/guides/language/language-tour#enumerated-types) | [in](https://dart.dev/guides/language/language-tour#for-loops) | [super](https://dart.dev/guides/language/language-tour#extending-a-class) |
| [async](https://dart.dev/guides/language/language-tour#asynchrony-support) | [export](https://dart.dev/guides/libraries/create-library-packages) | [interface](https://stackoverflow.com/questions/28595501/was-the-interface-keyword-removed-from-dart)  | [switch](https://dart.dev/guides/language/language-tour#switch-and-case) |
| [await](https://dart.dev/guides/language/language-tour#asynchrony-support)  | [extends](https://dart.dev/guides/language/language-tour#extending-a-class) | [is](https://dart.dev/guides/language/language-tour#type-test-operators) | [sync](https://dart.dev/guides/language/language-tour#generators)  |
| [break](https://dart.dev/guides/language/language-tour#break-and-continue) | [external](https://stackoverflow.com/questions/24929659/what-does-external-mean-in-dart)  | [library](https://dart.dev/guides/language/language-tour#libraries-and-visibility)  | [this](https://dart.dev/guides/language/language-tour#constructors) |
| [case](https://dart.dev/guides/language/language-tour#switch-and-case) | [factory](https://dart.dev/guides/language/language-tour#factory-constructors)  | [mixin](https://dart.dev/guides/language/language-tour#adding-features-to-a-class-mixins)  | [throw](https://dart.dev/guides/language/language-tour#throw) |
| [catch](https://dart.dev/guides/language/language-tour#catch) | [false](https://dart.dev/guides/language/language-tour#booleans) | [new](https://dart.dev/guides/language/language-tour#using-constructors) | [true](https://dart.dev/guides/language/language-tour#booleans) |
| [class](https://dart.dev/guides/language/language-tour#instance-variables) | [final](https://dart.dev/guides/language/language-tour#final-and-const) | [null](https://dart.dev/guides/language/language-tour#default-value) | [try](https://dart.dev/guides/language/language-tour#catch) |
| [const](https://dart.dev/guides/language/language-tour#final-and-const) | [finally](https://dart.dev/guides/language/language-tour#finally) | [on](https://dart.dev/guides/language/language-tour#catch)  | [typedef](https://dart.dev/guides/language/language-tour#typedefs)  |
| [continue](https://dart.dev/guides/language/language-tour#break-and-continue) | [for](https://dart.dev/guides/language/language-tour#for-loops) | [operator](https://dart.dev/guides/language/language-tour#overridable-operators)  | [var](https://dart.dev/guides/language/language-tour#variables) |
| [covariant](https://dart.dev/guides/language/sound-problems#the-covariant-keyword)  | [Function](https://dart.dev/guides/language/language-tour#functions)  | [part](https://dart.dev/guides/libraries/create-library-packages#organizing-a-library-package)  | [void](https://medium.com/dartlang/dart-2-legacy-of-the-void-e7afb5f44df0) |
| [default](https://dart.dev/guides/language/language-tour#switch-and-case) | [get](https://dart.dev/guides/language/language-tour#getters-and-setters)  | [rethrow](https://dart.dev/guides/language/language-tour#catch) | [while](https://dart.dev/guides/language/language-tour#while-and-do-while) |
| [deferred](https://dart.dev/guides/language/language-tour#lazily-loading-a-library)  | [hide](https://dart.dev/guides/language/language-tour#importing-only-part-of-a-library)  | [return](https://dart.dev/guides/language/language-tour#functions) | [with](https://dart.dev/guides/language/language-tour#adding-features-to-a-class-mixins) |
| [do](https://dart.dev/guides/language/language-tour#while-and-do-while) | [if](https://dart.dev/guides/language/language-tour#if-and-else) | [set](https://api.dart.dev/stable/dart-core/Set-class.html)  | [yield](https://dart.dev/guides/language/language-tour#generators)  |

