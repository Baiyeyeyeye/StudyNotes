# Kotlin学习

# Ch2 基本语法



### 函数

```kotlin
fun sum(x: Int, y: Int): Int{return x + y}
fun sum(x: Int, y: Int) = return x + y
```



Tips:

1. 一般函数**返回值**都需要显示指定；
2. 函数参数都需要指定





###  var与val

```kotlin
val book = Book()
```

book是指向堆中该对象的引用，val代表引用本身不可变，但引用指向的对象可变。

若将引用理解为对象实体的地址变量，则地址变量本身不可变，但目的地的对象可变。



### 函数式编程

函数可以像变量一样传来传去，或者说函数本身就被当成了复杂组合的基本元素。可以将函数作为参数传入到一个函数中。

函数类型就类似于我们当时解释器做的sml语言：

(参数类型列表) -> 返回值类型

```kotlin
(Int, String) -> Int
() -> Int
//也可以给参数取名字
(name: String, code: Int) -> Unit
//在类型后加上?代表可选

//参数类型和返回值也可设定为另一个函数类型：
((Int)-> Int) -> Int //参数为函数类型
()  -> ((Int) -> Int) //返回值为函数类型
```









