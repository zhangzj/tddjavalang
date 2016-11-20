# java核心技术

java语言本身有哪些语法，都有哪些方面需要了解，对应开发中的什么问题？

## 前言

java的高级特性；OOP，异常，反射代理，泛型，接口内部类，集合框架，事件监听器模型，并行；更高级的特性，文件与流，数据库，分布式对象，高级GUI，本地方法，国际化，XML，JavaBeans，网络，注释，高级图形；

## 1 Java程序设计概述

## 2 Java程序设计环境

安装JDK是开始学习Java的第一步，开发环境；设定环境变量，确保HelloWorld

### 2.3 使用命令行工具

javac；java

### 使用IDE

Eclipse，IDEA

## 3 Java的基本程序设计结构

java程序的基本结构，字符串，注释，数据类型，变量，运算符，输入输出，控制流，大数值，数组；

### 数据类型

整型 int short long byte 浮点型 float double； char boolean

### 变量

变量初始化；常量

### 运算符

算术运算符；自增自减运算度；关系运算符和布尔运算符；位运算符；数学函数与数学常量；数值类型之间的转换；强制类型转换；运算符优先级和括号；枚举类型；

### 字符串

String；子串；字符串拼接；不可变字符串；检测字符串是否相等；空串与null串；charAt，代码点和代码单元；String的方法，字符串API；

使用Java的API文档查询可用的方法；使用StringBuilder来构建字符串；

### 输入输出

Scanner对象，读取输入；printf方法格式化输出；

文件输入输出，Scanner；

### 控制流程

块block作用域；条件语句，if；循环，while，dowhile，for；多重选择switch；终端控制流程语句，跳出循环，break，continue；

### 大数值

java.Math中有两个类，BigDecimal和BigInteger；

### 数组

基本类型数组，不是容器；foreach循环；数组初始化和匿名数组；数组拷贝；

命令行参数，也即是main函数中的String[] args，命令行后面跟一个String的数组；

数组排序，工具类，Arrays表示数组相关的工具函数，Arrays.sort()；

多维数组；

## 4 对象与类

### 类

OOP，对象构造，预定义类，包，用户自定义类，类路径，静态域和静态方法，文档注释，方法参数，类设计技巧；

类是构造对象的模板或者蓝图；对象是由类构造而来；对象之间的区别使用对象引用来区别；类之间的关系有依赖，聚合，继承；依赖是使用一个类，聚合是包含一个类，继承是属于一个类；

### 使用预定义的类，现成的类

对象与对象变量；JDK中的Date和GregorianCalendar类；

setter和getter方法；

### 用户自定义类

源代码放到多个源文件中；构造器

基于类的访问权限，类中的多有方法中的代码可以访问类中所有的私有域；

final，表示必须被初始化，并且不可以被修改；

### 静态域和静态方法

static，静态表示是类级别的域，一个类只有一份；

静态常量表示类级别的全局常量；静态方法也是类级别，表示不能对对象使用的方法；

工厂方法，main方法

### 方法参数

传值调用，传值调用，java都是按引用调用；

### 对象构造

构造器重载；默认域初始化；无参构造器；显式域初始化；参数名字；构造器中调用另一个构造器；初始化块

对象析构和finalize方法，java中不需要自己管理回收对象，有GC；

### 包

package，保证类名的唯一性，类的命名就不会冲突，使用包管理类的布局的话；

导入类，import语句；静态导入，import static可以直接到与静态方法和静态域；

包作用域，没有访问权限修饰符，public private之类的东西，就是包访问权限，在同一个包中可见；

### 类路径

类存储在文件系统的子目录中，类的路径必须与包名匹配；classpath

### 文档注释

javadoc，由源文件生成一个html文档；

各级文档注释中有一些注解可以标记生成文档的信息；

### 类设计技巧

保证数据是private；一定对数据初始化；不要在类中使用过多的基本类型；不是所有的域都需要setter和getter；太臃肿的类要进行肢解，分解多个类；合适的类名和类方法，以体现职责；

## 5 继承

类，超类，子类；参数变量可变的方法；Object，所有类的超类；枚举类；泛型数组列表；反射；对象包赚器和自动装箱；继承设计技巧；