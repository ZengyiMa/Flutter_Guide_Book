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

下面为 Dart 内建的关键字

 

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

## 变量

这是创建变量并初始化它的示例:

```dart
var name = 'Bob';
```

变量存储引用。 名为 name 的变量包含对 String 对象的引用，其值为 “Bob”。 name 变量的类型推断为 String，但您可以通过指定它来更改该类型。 

如果对象不限于单个类型，请指定 Object 或 dynamic 动态类型，

```dart
dynamic name = 'Bob';
```

另一种选择是显式声明将推断出的类型

```dart
String name = 'Bob';
```

### 默认值

未初始化的变量的初始值为null。 即使是具有数字类型的变量最初也是null，因为数字也是对象。

```dart
int lineCount;
assert(lineCount == null);
```

### Final 和 const 关键字

如果您从不打算更改变量，请使用 final 或 const，而不是 var 或者其他类型。 final 变量只能设置一次，const变量是编译时常量，const变量是隐式 final 变量（不可变）

以下是创建和设置 final 变量的示例：

```dart
final name = 'Bob'; // Without a type annotation
final String nickname = 'Bobby';
```

您无法更改 final 变量的值：

```dart
name = 'Alice'; // Error: a final variable can only be set once.
```

将 const 用于您**编译时常量**。 如果 const 变量在类级别，则将其标记为static const。 在声明变量的地方，将值设置为**编译时常量**

例如数字或字符串文字，const变量或对常数进行算术运算的结果：

```dart
const bar = 1000000; // Unit of pressure (dynes/cm2)
const double atm = 1.01325 * bar; // Standard atmosphere
```

const 关键字不仅用于声明常量变量。 您还可以使用它来创建常量值，以及声明创建常量值的构造函数。 任何变量都可以具有常量值。

```dart
var foo = const [];
final bar = const [];
const baz = []; // Equivalent to `const []`
```

您可以更改非 final，非 const 变量的值，即使它曾经有一个 const 值：

```dart
foo = [1, 2, 3]; // Was const []
```

您无法更改 const 变量的值：

```dart
baz = [42]; // Error: Constant variables can't be assigned a value.
```





