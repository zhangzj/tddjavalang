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

### 类 超类 子类

继承链；继承的层次一级级形成链条，

多态，动态绑定，

阻止继承，final类和方法，final class可以阻止这个类别继承，如果一个方法有final修饰就不能被子类覆盖

强制类型转换，

抽象类；protected

### Obejct 所有类的超类

equals方法，检测一个对象是不是等于另一个对象；

hashcode方法，由对象生成的一个散列整型值，没有规律；

toString方法；

### 泛型数组列表

ArrayList泛型

### 对象包装器与自动装箱

### 参数数量可变 变参方法

### 枚举类

### 反射

在运行中分析类的能力；在运行中查看对象；实现通用的数组操作代码；利用Method对象

class类；捕获异常；利用反射分析类的能力，java.lang.reflect包中的三个类，Field，Method，Constructor分别用于描述类的域，方法和构造器；

运行时使用反射分析对象；

### 继承设计的技巧

把公共操作和域放在超类

不要使用protected域

使用继承实现is-a关系

除非所有继承的方法都有意义，否则不要使用继承

覆盖方法的时候不要改变预期行为

使用多态而不是类型信息

不要过多使用反射

## 6 接口与内部类

接口；内部类；对象克隆；代理；接口与回调；

### 接口

### 对象克隆

clone方法

### 接口与回调

callback是一个常见的设计模式，这种模式中，可以指出某个特定事件发生时应该采取的动作，比如鼠标点击，定时执行等；

### 内部类

内部类是定义在另一个类中的类；需要内部类的原因；可以访问定义所在类的作用域中的数据，包括私有数据；内部类可以对同一个包中的其他类隐藏起来；想定义一个回调函数并且不想编写大量代码时候，使用匿名内部类比较便捷；

使用内部类访问对象状态；内部类的特殊语法规则；局部内部类；

由外部方法访问final变量；匿名内部类；

代理，可以再运行时创建一个实现了一组给定接口的新类；只有在编译时无法确定需要实现哪个接口时才有必要使用；

## 7 图形程序设计

Swing，2D图形，创建窗口框架，颜色，框架定位，文本实用特殊字体，组件中显示信息，显示图像；

## 8 事件处理

事件处理基础；鼠标事件；动作；AWT事件继承层次；

## 9 Swing用户界面组件

Swing MVC，布局管理概述；文本输入；选择组件；菜；复杂的布局管理；对话框；

## 10 部署应用程序和applet

jar；applet；java web start；应用程序首选项；

如何将程序打包部署到用户的计算机上；

### jar

使用zip格式压缩了打包的类文件和其他文件；

清单文件，manifest，位于jar文件中的特殊的meta-inf子目录中，记录一些meta信息，比如版本信息等等

可运行的jar文件；使用jar命令的e选项指定入口点

### 应用程序首选项存储

用户对于软件的配置，可以进行本地的保存，然后再运行的时候可以读取配置；先介绍一个把配置信息存在属性问加你中的传统方式，再介绍一个首选项API，可以提供更加健壮的方案；

属性映射，property map，存放键值对的数据结构，Properties

PreferenceAPI；针对Properties的不足（配置文件不能简单存放在主目录，windows没有主目录概念；而且多个java程序的配置文件有可能命名冲突）；Preference就好像一个实现透明的中心知识库

## 11 异常 断言 日志和调试

处理错误，捕获异常，使用异常机制的技巧，使用断言，日志，调试技巧，GUI程序拍错技巧，使用调试器；

编译时候的错误可以修正代码来进行除错，那么运行时候的错误情况怎么处理？回滚保存之后终止程序，给用户报错看上去是合理的处理方式，如果程序有自己的除错方式，出错之后进行某些自定义的处理实际上也不错；

一个try语句可以有多个catch对应，每一个catch使用一个不同的异常类型处理不同的错误

这里java自带的断言貌似没有什么用；日志有日志框架；调试问题一般使用日志调试；

## 12 泛型程序设计

为什么要使用泛型设计；使用泛型比胡乱使用Object变量然后进行类型转换要优雅；泛型的根本在于代码的重用，之前是变量为中心的重用，泛型就是变量类型也加入了重用的变化当中；在泛型设计出现之前，使用Object引用的数组实现的；这引发了两个问题，第一，使用传进来的对象需要进行类型的强制转换，第二，因为是使用Object引用，所以可以添加任何类型的对象进来，没有编译检查；

泛型设计分为三个能力级别，基本级别只是使用泛型，不用考虑工作方式和原因；

定义简单泛型类；

类型参数跟在class名字的后面，使用尖括号括起来，一般E表示元素，KV表示键值，TUS表示任意类型；

泛型方法；类型变量的限定；限定类型参数必须实现某个接口或者继承某个类的方式，确定传进来的类型有某个方法；

泛型代码和虚拟机；约束与局限性；实现泛型类的一些注意点和规则，实话讲，还没有到自定义泛型类的地步；

泛型类型的继承规则；通配符类型；可以指定某个类的子类或者某个类的超类作为类型参数；

反射和泛型；

## 13 集合

集合接口；接口和实现的分离，ADT成为接口表示功能；迭代器帮助迭代集合中的所有元素；

具体的集合；链表等具体的ADT实现的JDK类库；

集合框架；包含很多接口和抽象类；集合的批量操作；传统数组和集合之间的转换；

算法；使用泛型来编写算法可以很大程度上提高代码重用性；

遗留的集合；Java问世以来的集合类，hashtable，属性映射表，properites；

## 14 多线程

多线程程序在较低的层次上扩展了多任务的概念，一个程序同时执行多个任务，每一个任务称为一个线程；线程和进程的区别在于进程有自己的变量上下文，线程之间是共享数据的；

什么是线程；使用Runnable对象的参数构建一个thread然后执行；

中断线程；要是run方法中的代码执行结束，或者出了异常，线程就会终止，还有一个强制终止线程的方法对一个线程调用interrupt方法，将中断状态置位；

线程状态；new,Runnable,blocked,waiting,timed waiting,terminated

线程属性；线程优先级，守护线程，未捕获异常处理器

同步；竞争状况，race condition，共享数据的存取冲突；锁对象，sychronized；条件对象；监视器；final变量；原子性；死锁

阻塞队列；线程安全的集合；Callable和Future；执行器；同步器；线程与Swing；

## 1 流与文件

流；读入字节的称为输入流，InputStream，可以写入一个字节序列的对象称作输出流，OutpuStream；流家族，

文本输入和输出；写出文本，读入文本，文本格式存储对象，字符集；

读入和写出二进制数据；
ZIP文档；
对象流与序列化；使用特殊格式保存对象，对象类需要实现Serializable接口；
使用文件；Path，Files，访问操作本地的文件系统；ZIP文件系统操作；
内存映射文件；文件系统映射到内存中，操作更快；文件加锁；
正则表达式；

## 2 XML

XML概述；
解析XML文档；DOM模型，
验证xml文档；自动校验文档是否有一个正确的结构；DTD，Schema
使用xpath来定位信息；
使用命名空间；
流机制解析器；文件很大的时候，可以再运行时解析节点，一部分一部分来；
生成xml文档；
xsl转换；XSLT机制可以指定将XML文档转换为其他格式的规则，比如纯文本，XHTML或者其他的XML格式

## 3 网络

连接到服务器；telnet，套接字超时Socket；IP地址，
实现服务器；套接字服务器，
可中断套接字；
获取web数据；URL和URI，URLConnection；
发送email；SMTP协议，javamail；

## 4 数据库编程

jdbc的设计；jdbc和微软的odbc思想相似，根据api编写的程序都可以与驱动管理器进行通信，而驱动管理器则通过与驱动程序与实际的数据库进行通信；
结构化查询语言；SQL语言
jdbc配置；数据库URL，DB驱动文件JAR文件，
执行sql语句；
执行查询操作；预备语句，preparedstatement；blob二进制大对象；sql转义，将标准sql转成特定数据库语言；
可滚动和可更新的结果集；
行集；
元数据；jdbc还可以提供关于数据库和表结构的详细信息；
事务；一组语句组成一个事务，transaction，所有语句顺利执行后，事务被提交，commit，如果中间有个语句出错，那么事务将会被回滚，好像没有语句执行过一样，来保证数据库的完整性；
web和企业应用中的连接管理；JNDI服务来定位数据源

## 5 国际化

国际化不仅仅是提供不同的文字语言，不同地方的日期时间，金融显示，数字都不一样；

Locales；
数字格式；
日期和时间；
排序；不同语言中的字母排序结果不一样；
消息格式化；MessageFormat类，
文本文件和字符集；
资源包；
一个完整的例子；

## 6 高级Swing

列表；JList；
表格；JTable；
树；文件系统，JTree；
文本构件；text控件；
进度指示器；进度条，ProgressMonitor；
构件组织器和装饰器；控件容器

## 7 高级AWT

绘图制作流程；
形状；
区域；
笔划；
着色；
坐标变换；
剪切；
透明与组合；
绘图提示；
图像读取器和写入器；
图像处理；
打印；
剪贴板；
拖放操作；
平台集成；

## 8 JavaBean构件

这里的bean是前端的组件，不是后端的bean；

为何使用Bean；
编写Bean的过程；
使用Bean来构造一个应用；
Bean属性与事件的命名模式；
Bean属性的类型；
Beaninfo类；
属性编辑器；
定制器；
JavaBean持久化；

## 9 安全

java提供了三种确保安全的机制；

语言设计特性，对数组的边界检查，无不受检查的类型转换，无指针算法等；访问控制机制，文件访问，网络访问等；代码签名，利用加密算法认证java代码，知道是不是被动过；

类加载器；将类加载到虚拟机的时候检查类的完整性；
字节码校验；
安全管理器与访问权限；
用户认证；
数字签名；
代码签名；
加密；

## 10 脚本 编译与注解处理

本章介绍了三种用于处理代码的技术，脚本API可以调用js或者Groovy脚本；可以在java程序内部编译java代码；注解处理器可以再包含著姐的java源码和类文件上进行操作；

**Java平台脚本；**

可以再java平台中选定一个引擎解释器，然后执行对应的的脚本；

可以获取的脚本引擎，构造一个ScriptEngineManager，

**编译器API；**

编译Java代码的Java程序；很多应用场景，比如开发环境，Java的教学辅助环境，自动化构建和测试工具；处理代码的模板工具，如JSP；

对编译过程的更多控制；比如代码的来源，类文件的存储位置等

**使用注解；**

注解出现在代码中，对应某一个处理工具对文件进行一些处理；没有处理工具对应，注解本身没什么用；

注解语法；

使用@interface声明一个注解，实际上就是一个java接口；
标准注解；用于编译的注解，@deprecated，@override等；用于管理资源的注解，注入资源@resource；元注解，注解注解的注解，@Target，@Retention，

源码级注解处理；简化编程模型，比如bean，使用@property来注解一个属性的setter和getter；

字节码工程；在字节码级别上设置注解；类加载器JIT技术

## 11 分布式对象

两个JVM之间使用RMI协议进行通信；

客户与服务器角色；

web中仅限于使用http协议，响应使用html；使用代理机制来搞定响应解析之类的事情；客户端类只进行一般的方法调用；

代理通信的实现技术使用；corba，使用二进制通信协议IIOP；web服务架构协议集，soap的xml通信；RMI，java远程方法调用技术

远程方法调用；

把参数传输到另一台机器上，调用那边对象的方法，传回结果；

![](http://ww1.sinaimg.cn/large/8d6a2535gw1fa352rstkzj20iu0efac3.jpg)

RMI编程模型；

远程方法接口模型，远程对象的接口必须扩展Remote接口，异常抛出也要是RemoteException；

RMI注册表，查找某个机器上的注册表，看看都有什么对象可用；返回存根之后，根据存根对象调用远程方法；

远程方法中的参数与返回值；

远程对象激活；激活机制允许延迟构造远程对象，第一次调用的时候再构造；

## 12 本地方法

如非必要，比如某个部分是其他语言编写的，就需要为支持每一个平台都提供一个单独的本地类库；尽量不要使用本地方法污染程序；使用本地方法的场景；应用需要访问的系统特性和设备通过java无法实现；已经有大量现成的代码，并且是全平台的；java的代价成本要比其他语言大很多；

Java的本地C代码互操作的API，JNI，java本地接口；

从Java程序中调用C函数；

数值参数与返回值；
字符串参数；
访问域；
编码签名；
调用Java方法；
访问数组元素；
错误处理；
使用调用API；
访问Windows注册表；
