## 并发

线程机制，允许同时进行多个活动，并发设计要比单线程的设计难很多

### 66 同步访问共享的可变数据

关键字synchronized可以保证在同一个时刻，只有一个线程可以执行某一个方法，或者一个代码块，这样子可以理解成互斥的一个方式；
