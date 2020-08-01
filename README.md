# dart-basic
Dart语言基础，创建于20200726
## Dart基础
### 第一章、开始
> main () 程序方法入口

### 第二章、数据类型
> `num`
+ 1.int 和 double是num 的父类
+ 2.floor 向下取整
+ 3.ceil 向上取整
+ 4.0.0 /0.0 NaN
+ 5.round 四舍五入
+6.~/ 除法取整

>  `var final const`

+ 1.使用var申明变量，可赋予不同类型的值
+ 2.var 申明变量未初始化时为 null
+ 3.final 申明一个只能赋值一次的变量
+ 4.使用const申明一个常量
+ 5.使用const申明的必须是编译期常量)

> `String`

+ 1.三个单引号或者双引号可输出多行文本
+ 2.\n 换行 \t tab
+ 3.引号前面加 r 不转义
+ 4.两个字符串相比较 == 比较的是内容
+ 5.差值表达式 ${} 只有一项的时候可以省略括号
+ 6.str * 10 字符串复制
+ 7.endsWith 是否以什么结束
+ 8.startWith 是否以什么结束
+ 9.split 以什么分隔，得到的是一个数组

> `bool`
>(true false)

> `List`
+ 1.在dart中数组和List是一样的概念
+ 2.indexOf() 查找元素所在位置，找到返回元素所在下标，没有找到则返回-1
+ 3.sort() 排序参数支持排序规则的方法 默认按照ascii码表排序
+ 4.add() 添加一个元素5. insert(index,value) 插入指定位置的元素
+ 6.forEach() 参数为一个方法 List 遍历
+ 7.不可变List List list = const [])

> `Map`
+ 1.Map的key value 可以是任意类型
+ 2.length
+ 3.isEmpty
+ 4.isNotEmpty
+ 5.keys 得到所有的key _CompactIterable<dynamic>
+ 6.values 得到所有的value  _CompactIterable<dynamic>
+ 7.containsKey('')  containsValue('')
+ 8.remove() //参数为key
+ 9.List 转 Map 默认会以下标为key list的内容为value 下标从零开始10. forEach() \\参数为一个方法 使用见代码)

> `dynamic`
> 动态数据类型

### 第三章、运算符

> `算数运算符`
  + \+
  + \-
  + \*
  + \/
  + ~/ 除法取整
  + % 求余数
  + ++
  + --

> `逻辑运算符`

  + !
  + &&
  + ||
  
>  `赋值运算符`

  + ==
  + ?== 当前者为null时执行后面
  + +=
  + -=
  + *=
  + /= 被除数需要是double类型
  + ~/= ~/
 
> `关系运算符`

 + \>
 + <
 + =
 + ==
 + \>=
 + <=
 + !=
 + 两个字符串比较 == 比较的是内容
 
>   `条件运算符`

 + ? 正常三木运算符
 + ?? 前者为空执行后者
 
 ### 第三章、控制语句
 
 > `if`
  + 和其他语言一致
  
 > `for for in `
  + 和其他语言一致
  
>` while 、do while `
   + 和其他语言一致
   
> `switch case`
  + 1.比较类型： num ,String ,编译器常量，对象，枚举
  + 2.非空case必须有一个break;
  + 3.default处理默认情况
  + 4.continue跳转
  + 5.可以加标签跳转，用法看代码
   
> `break continue`
   + 和其他语言一致 
   
### 第三章、方法

> `Funtion {} [] 可选位置参数、可选命名参数、参数默认值`
  + 1.在Dart中方法也是对象，并且有具体的类型Function
  + 2.返回值类型、参数类型都可以省略
  + 3.箭头语法 => expr  是{return expr;}的缩写。只适用于一个表达式
  + 4.方法都有返回值，如果没有指定默认返回一个null
  + 5.箭头语法不能写rerun
  + 6.三目运算可以写箭头语法
  + 7.可选参数： {} 可选命名参数 []可选位置参数
  + 8.必须参数只能放在第一，可选参数放在后面
  + 9.使用 = 在可选参数指定默认值，默认值只能是编译期的常量
  + 10.可选参数默认值：没有传递参数的时候使用，传递参数时则使用传递的参数
  + 11.方法对象：方法可以作为对象赋值给其他变量，方法可以作为参数传递给其他方法
  
 > `方法对象`
   + 1.方法对象：方法可以作为对象赋值给其他变量，方法可以作为参数传递给其他方法
   + 2.当将方法作为变量赋值时。写方法名称即可，变量加小括号调用
   + 3.当将方法作为参数传递的时候，也是写明方法名称即可。注意不能使用可选命名参数
   
 > `匿名方法`


 > `闭包`