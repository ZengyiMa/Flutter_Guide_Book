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

## 内建类型

### Numbers

数字类型：包含了2种类型：int 和 double

下面是一些使用示例

```dart
var x = 1;
var hex = 0xDEADBEEF;
double z = 1;

// 转换代码
// String -> int
var one = int.parse('1');
assert(one == 1);

// String -> double
var onePointOne = double.parse('1.1');
assert(onePointOne == 1.1);

// int -> String
String oneAsString = 1.toString();
assert(oneAsString == '1');

// double -> String
String piAsString = 3.14159.toStringAsFixed(2);
assert(piAsString == '3.14');
```

### Strings

字符串类型（UTF-16编码）

使用示例

```dart
// 基本用法
var s1 = 'Single quotes work well for string literals.';
var s2 = "Double quotes work just as well.";
var s3 = 'It\'s easy to escape the string delimiter.';
var s4 = "It's even easier to use the other delimiter.";
var s = 'string interpolation';
var s1 = 'String '
    'concatenation'
    " works even over line breaks.";
    
// 使用+来拼接字符串
var s2 = 'The + operator ' + 'works, as well.';
assert(s2 == 'The + operator works, as well.');

// 多行文本
var s1 = '''
You can create
multi-line strings like this one.
''';

var s2 = """This is also a
multi-line string.""";

// 原始字符串
var s = r'In a raw string, not even \n gets special treatment.';
```

更详细的内容请查看：[https://dart.dev/guides/libraries/library-tour\#strings-and-regular-expressions](https://dart.dev/guides/libraries/library-tour#strings-and-regular-expressions)

### Booleans

为了表示布尔值，Dart 有一个名为 bool 的类型。 只有两个对象具有bool类型：boolean 字面值 true 和 false，它们都是编译时常量。

 Dart的类型安全意味着您不能使用if（非 bool 型）或assert（非 bool 型）之类的代码。 相反，明确检查值，如下所示：

```dart
// Check for an empty string.
var fullName = '';
assert(fullName.isEmpty);

// Check for zero.
var hitPoints = 0;
assert(hitPoints <= 0);

// Check for null.
var unicorn;
assert(unicorn == null);

// Check for NaN.
var iMeantToDoThis = 0 / 0;
assert(iMeantToDoThis.isNaN);
```

### Lists

也许几乎每种编程语言中最常见的集合是数组或有序的对象组。 在 Dart 中，数组是 List 对象，因此大多数人只是将它们称为 lists。

Dart 列表 字面看起来像 JavaScript 数组符号。 这是一个简单的 Dart 列表：

```dart
var list = [1, 2, 3];
```

列表使用从零开始的索引，其中0是第一个元素的索引，`list.length - 1` 是最后一个元素的索引。 您可以获得列表的长度并像在 JavaScript 中一样引用列表元素：

```dart
var list = [1, 2, 3];
assert(list.length == 3);
assert(list[1] == 2);

list[1] = 1;
assert(list[1] == 1);
```

要创建一个编译时常量的列表，请在列表之前添加const：

```dart
var constantList = const [1, 2, 3];
// constantList[1] = 1; // Uncommenting this causes an error.
```

例如，您可以使用扩展运算符（...）将列表的所有元素插入另一个列表：

```dart
var list = [1, 2, 3];
var list2 = [0, ...list];
assert(list2.length == 4);
```

如果扩展运算符右侧的表达式可能为null，则可以通过使用支持null的扩展运算符（...？）来避免异常：

```dart
var list;
var list2 = [0, ...?list];
assert(list2.length == 1);
```

Dart 2.3还引入了 if 和 collection 的集合，您可以使用它来使用条件（if）和重复（for）来构建集合。

这是一个使用示例，如果要创建一个包含三个或四个项目的列表：

```dart
var nav = [
  'Home',
  'Furniture',
  'Plants',
  if (promoActive) 'Outlet'
];
```

这是一个使用集合来操作列表项目然后将它们添加到另一个列表之前的示例：

```dart
var listOfInts = [1, 2, 3];
var listOfStrings = [
  '#0',
  for (var i in listOfInts) '#$i'
];
assert(listOfStrings[1] == '#1');
```

### Sets

Dart中的 set 是一组无序的唯一元素。 对集合的 Dart 支持由 Set 字面符和 Set 类型提供。

这是一个简单的 Dart set，使用set 字面符创建：

```dart
var halogens = {'fluorine', 'chlorine', 'bromine', 'iodine', 'astatine'};
```

### Maps

通常，map 是关联键和值的对象。 键和值都可以是任何类型的对象。 每个键只出现一次，但您可以多次使用相同的值。 Dart 支持由 Map 字面符和 Map 类型提供。

这里有几个简单的Dart Map示例，使用 Map 字面符创建：

```dart
var gifts = {
  // Key:    Value
  'first': 'partridge',
  'second': 'turtledoves',
  'fifth': 'golden rings'
};

var nobleGases = {
  2: 'helium',
  10: 'neon',
  18: 'argon',
};
```

您可以使用Map构造函数创建对象：

```dart
var gifts = Map();
gifts['first'] = 'partridge';
gifts['second'] = 'turtledoves';
gifts['fifth'] = 'golden rings';

var nobleGases = Map();
nobleGases[2] = 'helium';
nobleGases[10] = 'neon';
nobleGases[18] = 'argon';
```

像在 JavaScript 中一样，将新的键值对添加到现有 Map：

```dart
var gifts = {'first': 'partridge'};
gifts['fourth'] = 'calling birds'; // Add a key-value pair
```

和 JavaScript 中相同的方式从 Map 中检索值：

```dart
var gifts = {'first': 'partridge'};
assert(gifts['first'] == 'partridge');
```

如果您查找不在 Map 中的键，则会得到 null 作为返回值：

```dart
var gifts = {'first': 'partridge'};
assert(gifts['fifth'] == null);
```

使用 `.length` 来获取 Map 中键值对的数量：

```text
var gifts = {'first': 'partridge'};
gifts['fourth'] = 'calling birds';
assert(gifts.length == 2);
```

要创建一个编译时常量的 Map ，请在map 字面符之前添加const：

```text
final constantMap = const {
  2: 'helium',
  10: 'neon',
  18: 'argon',
};

// constantMap[2] = 'Helium'; // Uncommenting this causes an error.
```

### Runes

在 Dart 中，runes 是字符串的UTF-32代码点对象。

Unicode为世界上所有书写系统中使用的每个字母，数字和符号定义唯一的数值。 由于Dart字符串是 UTF-16 代码单元的序列，因此在字符串中表示32位 Unicode 值需要特殊语法。

表达Unicode代码点的常用方法是 uXXXX，其中 XXXX 是 4 位十六进制值。 例如，心符号（♥）是 u2665。 要指定多于或少于4个十六进制数字，请将值放在大括号中。 例如，笑的表情符号（😆）是 u {1f600}。

String类有几个属性可用于提取符文信息。 `codeUnitAt` 和 `codeUnit`属性返回16位代码单元。 使用runes属性获取字符串的符文。

```dart
main() {
  var clapping = '\u{1f44f}';
  print(clapping);
  print(clapping.codeUnits);
  print(clapping.runes.toList());

  Runes input = new Runes(
      '\u2665  \u{1f605}  \u{1f60e}  \u{1f47b}  \u{1f596}  \u{1f44d}');
  print(new String.fromCharCodes(input));
}
```

### Symbols

Symbol 对象表示 Dart 程序中声明的运算符或标识符。 您可能永远不需要使用符号，但它们对于按名称引用标识符的API非常有用，因为缩小会更改标识符名称而不会更改标识符符号。

要获取标识符的符号，请使用符号文字，它只是＃后跟标识符：

```dart
#radix
#bar
```

## Functions



