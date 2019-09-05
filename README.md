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
- 异常错误的分类
- 常见异常，自定义异常
- 注解的使用
- java新版本新特性

### 2. 集合
- List、map、Set各个实现类的底层原理等等，优缺点等
- 用过哪些map类，map的存储方式，存储结构，hashcode,扩容，默认值等
- map的线程安全方面有哪些处理，ConcurrentHashMap与hashmap具体哪里不同
- JAVA8的ConcurrentHashMap为什么放弃了分段锁，有什么问题吗，如果你来设计，你如何设计
- 有没有有序的map，怎么实现的
- ArrayList、LinkedList、Hashtable、HashMap、ConcurrentHashMap、HashSet的实现原理，能流利作答，当然能掌握CopyOnWrite容器和Queue是再好不过的了
- HashMap，源码级别，为什么线程不安全，哈希冲突的常见解决
### 3. 设计模式
- 设计模式的基本概念与原理
- 23中设计模式的优缺点，实现方式，适用场景

### 4. 多线程并发

#### 线程基础
- 基础的线程知识
- 导致线程死锁的原因？怎么解除线程死锁。
- 什么是多线程并发和并行
- 什么是线程安全问题
- 共享变量的内存可见性问题
- 多线程的实现方式
- 线程的状态
- sleep和wait的区别
- sleep和sleep(0)的区别
- wait和notify同步，源代码分析
- 多线程线程挂住了怎么办，案例分析
- 指令重排序
- 什么是伪共享,为何会出现，以及如何避免？
- CAS机制是什么，如何解决ABA问题
- Volatile关键字的内存语义是什么？
- Synchroniezd的原理，使用场景，使用synchronized修饰静态方法和非静态方法有什么区别
- Lock与Synchroniezd的区别
- 量级锁，可重入锁，公平锁，非公平锁，乐观锁，悲观锁，独占锁，共享锁
- ThreadLocal详解，用途，原理，注意事项
- InheritableThreadLocal 原理，InheritableThreadLocal 是如何弥补 ThreadLocal 不支持继承的特性？
- synchronized和ReentrantLock的区别、synchronized锁普通方法和锁静态方法、死锁的原理及排查方法等等

#### JUC包里的并发工具和集合
- countdowlatch和cyclicbarrier的内部原理和用法，以及相互之间的差别(比如countdownlatch的await方法和是怎么实现的)。
- CountDownLatch 与线程的 Join 方法区别是什么？
- Semaphore 的内部实现是怎样的？
- 原子类及其原理，AtomicLong的实现原理
- 独占锁 ReentrantLock 原理？
- 读写锁 ReentrantReadWriteLock 原理
- StampedLock 锁原理的理解使用？
- 回环屏障 CyclicBarrier 的理解使用？
- 读写锁的原理，还有使用场景
- 谈下对基于链表的非阻塞无界队列 ConcurrentLinkedQueue 原理的理解？
- ConcurrentLinkedQueue 内部是如何使用 CAS 非阻塞算法来保证多线程下入队出队操作的线程安全？、
- 基于链表的阻塞队列 LinkedBlockingQueue 原理。
- 阻塞队列LinkedBlockingQueue 内部是如何使用两个独占锁 ReentrantLock 以及对应的条件变量保证多线程先入队出队操作的线程安全？
- 对AbstractQueuedSynchronizer了解多少，讲讲加锁和解锁的流程，独占锁和公平所加锁有什么不同。
- 简述ConcurrentLinkedQueue和LinkedBlockingQueue的用处和不同之处。
- 延迟队列的实现方式，delayQueue和时间轮算法的异同
- 并发组件CopyOnWriteArrayList 是如何通过写时拷贝实现并发安全的 List？

#### 并发设计
- 线程池的原理，构造函数，源代码分析，具体场景分享，尝试实现一个简单的线程池
- 并发安全链表的设计
- 有哪些无锁数据结构，实现的原理是什么

- 非常多个线程（可能是不同机器），相互之间需要等待协调，才能完成某种工作，问怎么设计这种协调方案
- 多个线程怎么保证顺序执行，有哪些实现方式，如何保证多个线程执行完再拿取结果



### 5. IO
- IO模型有哪些，讲讲你理解的nio ，他和bio，aio的区别是啥，谈谈reactor模型。
- FILE IO
- 阻塞/非阻塞的区别、同步/异步的区别，借此理解阻塞IO、非阻塞IO、多路复用IO、异步IO这四种IO模型，Socket IO如何和这四种模型相关联。
- NIO
- 多路复用的概念

### 6.网络
- Socket交互流程，基础代码实现
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
- TCP协议，建立过程，慢启动，滑动窗口，七层模型
- 详解TCP三次握手和四次挥手的流程，为什么断开连接要4次,如果握手只有两次，会出现什么
- TIME_WAIT和CLOSE_WAIT的区别。
- TCP/IP 如何保证数据的可靠性，TCP头的结构
- 什么是TCP粘包，拆包。解决方式是什么
- webservice协议，（wsdl/soap格式，与restt办议的区别）？
- DNS解析过程
- 如何避免浏览器缓存
- 浏览器打开一个链接的时候，计算机做了什么

### 7. JDK源码
- 集合的实现代码
- 锁的实现代码，ReentrantLock、AQS的源代码
- AtomicInteger的实现原理，主要能说清楚CAS机制并且AtomicInteger是如何利用CAS机制实现的
- 线程池的实现代码
- Object的内容

### 8. Java虚拟机
- 各个区域的作用
- JVM每个区域的内存溢出，栈溢出的场景
- 内存模型，重排序，内存屏障，happen-before规则
- 垃圾收集算法
- 类加载器有哪些，双亲委派模型机制
- tomcat类加载机制
- 可以打破双亲委派吗，怎么打破
- 简述垃圾回收机制，垃圾回收器基本原理
- 判断一个对象是否存活，对象什么时候被垃圾回收
- 垃圾回收的优点，考虑两种回收机制
- 垃圾收集的几种方式
- JVM内存结构，Eden和Survivor比例，为什么分为新生代老年代，新生到为什么还要划分Eden和Survivor
- 各个不同类型的垃圾回收器的用法，优缺点，搭配，使用场景
- 一次完整的GC流程是什么，如何晋升老年代，说出几个重要的JVM参数
- Minor GC和Major GC简述
- 分布式垃圾回收
- volatile关键字使用规则
- 浅谈一些线上使用的JVM参数
- 内存泄露
- 虚拟机性能调优
- 线程的堆栈信息怎么得，JVM GC日志，dump文件分析
- 性能监控和故障处理工具
- 常见异步手段
### 9. 数据库
- sql语句，基础还有优化
- mysql结构
- 数据库性能优化，mysql性能调优
- JDBC
- 事务的理解
- 事务失败的场景，怎么解决
- 数据库的隔离级别，各自含义，mysql默认的隔离级别
- 什么是幻读
- MYSQL有哪些存储引擎，各自优缺点
- MYSQL锁并发
- 高并发下（红包），如何保证数据一致性，如何做到安全的修改同一行数据。
- 乐观锁和悲观锁是什么，INNODB的标准行级锁有哪2种，解释其含义
- SQL优化的一般步骤是什么，怎么看执行计划，如何理解其中各个字段的含义。
- 数据库举出来一个死锁例子，mysql怎么解决死锁
- MYsql的索引原理，索引的类型有哪些，如何创建合理的索引，索引如何优化。
- 聚集索引，非聚集索引的区别
- Btree什么时候分裂，怎么分裂怎么平衡
- 读写分离，分库分表
- 主从延时
- MYSQL监控
- 瓶颈分析

### 10. 数据结构和算法
- 空间复杂度，时间复杂度
- 数组，栈，链表等线性表，插入删除遍历操作
- 树的知识，遍历，各种常见的树的插入、删除、转化
- 图，图的遍历
- 常用的排序
- 寻址法
- 适用场景
- 不同数据结构经典范例
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
#### 13.1 分布式原理
- 分布式的演变
- 单机应用到分布式扩展
- 系统监控，容灾，存储动态扩容
- 架构设计及其业务驱动分化
- CAP、Base理论应用
- 最终一致性，怎么实现
#### 13.2 分布式架构策略

#### 13.3 分布式中间件

#### 13.4 分布式实战

#### 13.5 消息队列
- 消息队列的使用场景
- 消息的重发补充策略
- 消息有序性的保证
- 不同MQ之间的区别，优缺点，线程安全性
- MQ系统如何保证数据不丢失
- rabbitmq
- kafka
- 利用MQ实现最终一致性
- 消息延迟过期处理
#### 13.6 分布式缓存
- 分布式缓存和一致性哈希？
- 常见的缓存策略
- 一般的缓存系统，怎么设计
- 缓存击穿和雪崩，怎么防止
- 缓存数据的过期更新
- redis基础
- redis数据结构
- redis2和3区别，内部通讯机制
- redis的并发竞争问题，redis的CAS操作
- redis的选举算法，流程
- redis持久化 机制，aod和rdb区别
- redis集群 优劣，淘汰策略，怎么同步数据
- redis优化
- redis主从复制
- redis线程模型
- redis实现分布式锁
- redis缓存分片
- redis数据淘汰策略
- redis队列应用场景
- 设置一个可以控制缓存总大小的自适应本地缓存
- 本地缓存和集中式缓存的使用，优缺点
- Memcache基础
- redis和Memcache的区别

### 14. 微服务
- 微服务框架
- Spring Cloud
- Docker
- 微服务架构
### 15. 工程化内容
- Maven内容原理
- Maven生成jar
- Maven冲突解决，包依赖，问题定位解决
- Maven手写插件，流行插件

- Git内容原理
- Git冲突和解决
- Git团队案例
- Git规范

- Jenkins搭建自动部署环境
- Jenkins继承maven、git实现自动部署
- 多环境，权限配置

- Sonar代码质量管理介绍
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
### 17.性能优化
- 性能优化基准
- JVM调优
- Tomcat调优
- Mysql调优



