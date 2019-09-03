# someData
存放一些思维导图，图片，ppt等等

## Java知识点

### 1. 基本语法和对象概念，异常，反射等
- 关键字保留字的基本概念
- 基础类型用法，各自占据的字节
- 访问权限控制总结
- String类的研究，String可以被继承吗，为什么不可变，在虚拟机内存中是怎么存储的
- String，StringBuffer，StringBuilder的区别，多线程下的优缺点，从源代码分析
- 对象的三大特性
- 接口和抽象类的区别，使用场景
- 类的实例化顺序，当new执行的时候，父类静态数据，父类构造函数，字段，子类静态数据，子类的构造函数怎么执行的
- 继承和聚合的区别
- final的用途
- 深拷贝，浅拷贝的区别
- 自动装箱拆箱
- 如何在父类中为子类自动完成所有的hashcode和equals？优劣点在哪里，两者只实现其中一个会有什么影响
- 反射的原理，反射创建类实例的三种方式是什么。
- 反射中，Class.forName和ClassLoader区别
- 动态代理的几种实现方式，对应的优缺点
- 动态代理与cglib实现的区别
- 为什么CGlib方式可以对接口实现代理
- 序列化，反序列化
- java新版本新特性

### 2. 集合
- List、map、Set各个实现类的底层原理等等，优缺点等
- 用过哪些map类，map的存储方式，存储结构，hashcode,扩容，默认值等
- map的线程安全方面有哪些处理，ConcurrentHashMap与hashmap具体哪里不同
- JAVA8的ConcurrentHashMap为什么放弃了分段锁，有什么问题吗，如果你来设计，你如何设计
- 有没有有序的map，怎么实现的
- ArrayList、LinkedList、Hashtable、HashMap、ConcurrentHashMap、HashSet的实现原理，能流利作答，当然能掌握CopyOnWrite容器和Queue是再好不过的了

### 3. 设计模式
- 设计模式的基本概念与原理
- 23中设计模式的优缺点，实现方式，适用场景

### 4. 多线程
- 基础的线程知识
- 多线程的实现方式
- 线程的状态
- sleep和wait的区别
- sleep和sleep(0)的区别
- wait和notify同步，源代码分析
- 多线程线程挂住了怎么办，案例分析
- CAS机制是什么，如何解决ABA问题
- Lock与Synchroniezd的区别
- Synchroniezd的原理，使用场景，使用synchronized修饰静态方法和非静态方法有什么区别
- 量级锁，可重入锁，公平锁，非公平锁，乐观锁，悲观锁
- 原子类及其原理
- JUC包里的并发工具和原理
- 线程池的原理，构造函数，源代码分析，具体场景分享
- ThreadLocal详解，用途，原理，注意事项
- 并发安全链表的设计
- 有哪些无锁数据结构，实现的原理是什么
- countdowlatch和cyclicbarrier的内部原理和用法，以及相互之间的差别(比如countdownlatch的await方法和是怎么实现的)。
- 对AbstractQueuedSynchronizer了解多少，讲讲加锁和解锁的流程，独占锁和公平所加锁有什么不同。
- 简述ConcurrentLinkedQueue和LinkedBlockingQueue的用处和不同之处。
- 导致线程死锁的原因？怎么解除线程死锁。
- 非常多个线程（可能是不同机器），相互之间需要等待协调，才能完成某种工作，问怎么设计这种协调方案
- 读写锁的原理，还有使用场景
- 多个线程怎么保证顺序执行，有哪些实现方式，如何保证多个线程执行完再拿取结果
- 延迟队列的实现方式，delayQueue和时间轮算法的异同
- synchronized和ReentrantLock的区别、synchronized锁普通方法和锁静态方法、死锁的原理及排查方法等等

### 5. IO
- IO模型有哪些，讲讲你理解的nio ，他和bio，aio的区别是啥，谈谈reactor模型。
- FILE IO
- 阻塞/非阻塞的区别、同步/异步的区别，借此理解阻塞IO、非阻塞IO、多路复用IO、异步IO这四种IO模型，Socket IO如何和这四种模型相关联。
- NIO
- 多路复用的概念
- Netty

### 6.网络
- JAVA Socket
- 计算机网络分层
- 网络协议 Http，Tcp、IP
- HTTP1.0和HTTP1.1区别
- HTTP几种响应码
- HTTP协议的无状态性是什么
- HTTP请求get和set的区别以及数据包格式
- HTTP的method
- HTTP请求的报文格式
- HTTP长连接
- HTTP的加密方式，讲讲加密解密流程
- HTTP和HTTPS的三次握手有什么区别
- 分块传送
- session和cookie区别
- 详解TCP三次握手和四次挥手的流程，为什么断开连接要4次,如果握手只有两次，会出现什么
- TIME_WAIT和CLOSE_WAIT的区别。
- TCP/IP 如何保证可靠性，TCP头的结构
- 什么是TCP粘包，拆包。解决方式是什么
- 如何避免浏览器缓存
- 浏览器打开一个链接的时候，计算机做了什么

### 7. JDK源码
- 集合的实现代码
- 锁的实现代码，ReentrantLock、AQS的源代码
- AtomicInteger的实现原理，主要能说清楚CAS机制并且AtomicInteger是如何利用CAS机制实现的
- 线程池的实现代码
- Object的内容

### 8. Java虚拟机
- JVM每个区域的内存溢出，栈溢出的场景
- JVM内存结构，Eden和Survivor比例，为什么分为新生代老年代，新生到为什么还要划分Eden和Survivor
- 各个不同类型的垃圾回收器的用法，优缺点，搭配，使用场景
- 一次完整的GC流程是什么，如何晋升老年代，说出几个重要的JVM参数
- 内存模型，重排序，内存屏障，happen-before规则
- 垃圾收集算法
- 类加载器，可以打破双亲委派吗，怎么打破
- volatile关键字使用规则
- 浅谈一些线上使用的JVM参数
- 内存布局
- 虚拟机调优
- 线程的堆栈信息怎么得，JVM一些对应的文件怎么分析

### 9. 数据库
- sql语句，基础还有优化
- mysql结构
- 数据库性能优化，mysql性能调优
- JDBC
- 数据库的隔离级别，各自含义，mysql默认的隔离级别
- 什么是幻读
- MYSQL有哪些存储引擎，各自优缺点
- 高并发下，如何做到安全的修改同一行数据。
- 乐观锁和悲观锁是什么，INNODB的标准行级锁有哪2种，解释其含义
- SQL优化的一般步骤是什么，怎么看执行计划，如何理解其中各个字段的含义。
### 10. 数据结构和算法
- 空间复杂度，时间复杂度
- 数组，栈，链表等线性表
- 树的知识，
- 图
- 常用的排序
- 适用场景
- 10亿个数字里面找到最小的10个
- 1亿个数字，有2个重复，快速找到，时间空间最优化
- 2亿个随机生成的无序整数,找出中间大小的值。
- 给一个不知道长度的（可能很大）输入字符串，设计一种方案，将重复的字符排重。
- 有3n+1个数字，其中3n个中是重复的，只有1个是不重复的，怎么找出来
- 写一个字符串的反转函数
- 一个单向链表，删除倒数第N个数据。
- 一个已经构建好的TreeSet，怎么完成倒排序。
- 200个有序的数组，每个数组里面100个元素，找出top20的元素。
- 单向链表，查找中间的那个元素。
### 11. 操作系统
- 进程线程区别
- 操作系统中线程切换的过程
- linux的top命令详解
- linux的基本命令
- shell语法，能独自写脚本
- Linux下的IO模型
- epoll和poll有什么区别
- 一行命令输出正在运行的java进程
- 查看文件的最后5行
- 线上CPU飙升，怎么查找问题
- 在Linux下搭建服务器，维护

### 12. WEB
- web.xml内容
- servlet,listener,filter
- get/post
- 一些常用内容技巧1
- SOA，RPC
- tomcat原理学习
- 自己能手动搭建web框架
- 单点登录
- 权限管理

### 13. 分布式

### 14. 微服务

### 15. 工程化内容
- Maven内容原理
- Git内容原理

### 16. 开源框架
- tomcat结构，其类加载器流程，线程模型
- tomcat怎么调优，参数等等
- Spring的加载流程
- Spring AOP的实现原理
- Spring的事务传播属性
- Spring怎么管理事务，配置事务
- 说说你对Spring的理解，非单例注入的原理？它的生命周期？循环注入的原理，aop的实现原理，说说aop中的几个术语，它们是怎么相互工作的。
- Springmvc 中DispatcherServlet初始化过程
- springmvc用到的注解，作用是什么，原理
- springboot启动机制
- netty的线程模型，netty如何基于reactor模型上实现的
- netty的fashwheeltimer的用法，实现原理，是否出现过调用不够准时，怎么解决
- netty的心跳处理在弱网下怎么办
- netty的通讯协议是什么样的
- Mybatis，hibernate
- AOP等等



