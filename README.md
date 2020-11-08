# autumn_notes
preparations and notes

### 操作系统

- 必看内容：
    1. (3.3-4.5) 连续&非连续内存分配、分页、分段
    2. (5.1-5.5) 虚拟内存
    3. (6.1-6.10) 页面置换算法
    4. (7.1-7.14) 进程、线程
    5. (8.1-8.6) 调度算法
    6. (9.1-11.8) 进程同步方法、死锁、一些常见概念。嫌多可以看小土刀
    7. [小土刀操作系统总结](https://wdxtub.com/interview/14520847747820.html) 主要看进程vs线程、死锁、进程同步方法、中断、上下文切换、虚存、进程调度即可。其他的不是重点。
- 其他自用内容：
- [进程相关问题1](https://github.com/dabaitudiu/autumn_notes/blob/master/Operating%20System/7.%20%E8%BF%9B%E7%A8%8B%E4%B8%8E%E7%BA%BF%E7%A8%8B.md) &nbsp; &nbsp;[Source Video](https://www.bilibili.com/video/BV1js411b7vg?p=42)
- [基本概念](https://github.com/dabaitudiu/autumn_notes/blob/master/Operating%20System/2.%20%E5%9F%BA%E6%9C%AC%E6%A6%82%E5%BF%B5.md)
- [进程、线程](https://github.com/dabaitudiu/autumn_notes/blob/master/Operating%20System/1.%20%E8%BF%9B%E7%A8%8B%E7%BA%BF%E7%A8%8B.md)
- [CPU 100%如何排查](https://github.com/dabaitudiu/autumn_notes/blob/master/Operating%20System/cpu100.md)

### JVM
- 必看内容：JVM结构、类加载过程、垃圾回收(重点) 
    1. [JVM入门](https://coding.imooc.com/class/429.html) 看三~六章就够了，实践部分不用看，背理论即可。
    2. [CMS详解1](https://juejin.im/post/6844903782107578382)
    3. [CMS、G1详解](https://juejin.im/post/6844903922872614925)
    4. 这一部分很重要，必须熟练掌握。JVM结构，双亲委派，类加载各个过程，垃圾收集过程和算法必须背熟
- 自用：
- [类加载过程](https://github.com/dabaitudiu/autumn_notes/blob/master/JVM/3.%20%E7%B1%BB%E5%8A%A0%E8%BD%BD%E3%80%81%E8%BF%9E%E6%8E%A5%E3%80%81%E5%88%9D%E5%A7%8B%E5%8C%96.md)

### 多线程
- 多线程看悟空的这三门课，必看：[wukong](http://www.imooc.com/t/2854586)
    1. 先看线程八大核心+Java并发底层原理精讲 前两章
    2. 看免费课synchronized
    3. 看JUC那门， 看到CAS
    4. 这三门认真看完，所有多线程的问题全都秒
0. [Synchronized](https://github.com/dabaitudiu/autumn_notes/blob/master/Java%E5%A4%9A%E7%BA%BF%E7%A8%8B/0.Synchronized.md)
1. [创建线程](https://github.com/dabaitudiu/autumn_notes/blob/master/Java%E5%A4%9A%E7%BA%BF%E7%A8%8B/1.%E5%88%9B%E5%BB%BA%E7%BA%BF%E7%A8%8B.md)
2. [启动线程](https://github.com/dabaitudiu/autumn_notes/blob/master/Java%E5%A4%9A%E7%BA%BF%E7%A8%8B/2.%E5%90%AF%E5%8A%A8%E7%BA%BF%E7%A8%8B.md)
3. [停止线程](https://github.com/dabaitudiu/autumn_notes/blob/master/Java%E5%A4%9A%E7%BA%BF%E7%A8%8B/3.%E5%81%9C%E6%AD%A2%E7%BA%BF%E7%A8%8B.md)
4. [线程生命周期](https://github.com/dabaitudiu/autumn_notes/blob/master/Java%E5%A4%9A%E7%BA%BF%E7%A8%8B/4.%20%E7%BA%BF%E7%A8%8B%E7%94%9F%E5%91%BD%E5%91%A8%E6%9C%9F.md)
5. [线程相关方法](https://github.com/dabaitudiu/autumn_notes/blob/master/Java%E5%A4%9A%E7%BA%BF%E7%A8%8B/5.%20%E7%BA%BF%E7%A8%8B%E7%9B%B8%E5%85%B3%E6%96%B9%E6%B3%95.md)
6. [线程属性与异常处理](https://github.com/dabaitudiu/autumn_notes/blob/master/Java%E5%A4%9A%E7%BA%BF%E7%A8%8B/6.%E7%BA%BF%E7%A8%8B%E5%B1%9E%E6%80%A7%E4%B8%8E%E5%BC%82%E5%B8%B8%E5%A4%84%E7%90%86.md)
7. [线程安全](https://github.com/dabaitudiu/autumn_notes/blob/master/Java%E5%A4%9A%E7%BA%BF%E7%A8%8B/7.%E7%BA%BF%E7%A8%8B%E5%AE%89%E5%85%A8.md)
8. [Java内存模型](https://github.com/dabaitudiu/autumn_notes/blob/master/Java%E5%A4%9A%E7%BA%BF%E7%A8%8B/8.JMM.md)
9. [死锁](https://github.com/dabaitudiu/autumn_notes/blob/master/Java%E5%A4%9A%E7%BA%BF%E7%A8%8B/9.%E6%AD%BB%E9%94%81.md)
10. [线程池](https://github.com/dabaitudiu/autumn_notes/blob/master/Java%E5%A4%9A%E7%BA%BF%E7%A8%8B/10.%E7%BA%BF%E7%A8%8B%E6%B1%A0.md)
11. [ThreadLocal](https://github.com/dabaitudiu/autumn_notes/blob/master/Java%E5%A4%9A%E7%BA%BF%E7%A8%8B/11.%20ThreadLocal.md)
12. [锁](https://github.com/dabaitudiu/autumn_notes/blob/master/Java%E5%A4%9A%E7%BA%BF%E7%A8%8B/12.%20%E9%94%81.md)
14. [CAS](https://github.com/dabaitudiu/autumn_notes/blob/master/Java%E5%A4%9A%E7%BA%BF%E7%A8%8B/14.%20CAS.md)
15. [Immutable](https://github.com/dabaitudiu/autumn_notes/blob/master/Java%E5%A4%9A%E7%BA%BF%E7%A8%8B/15.%20Immutable.md)
16. [并发容器](https://github.com/dabaitudiu/autumn_notes/blob/master/Java%E5%A4%9A%E7%BA%BF%E7%A8%8B/16.%20%E5%B9%B6%E5%8F%91%E5%AE%B9%E5%99%A8.md)

### 数据库
- 我的弱项，也没什么特别好的建议，内容太多，只给一些参考：
    1. [剑指java面试offer](https://coding.imooc.com/class/303.html)数据库那一章，当入门
    2. [全技术栈企业级性能调优万花筒](https://coding.imooc.com/class/442.html)第3~第6章。不看也行，看了心里有底。
- 自用：
- [MySQL45讲](https://time.geekbang.org/column/intro/139)
- [Innodb中的事务隔离级别和锁的关系](https://tech.meituan.com/2014/08/20/innodb-lock.html) (必看)
- [MySQL中的MVCC](https://blog.csdn.net/waves___/article/details/105295060)(弥补上面那篇MVCC讲的不好的部分)
- [MySQL中各种锁的实现](https://tonydong.blog.csdn.net/article/details/103324323)
- [redo,undo的对比](https://www.infoq.cn/article/M6g1yjZqK6HiTIl_9bex)
- [MySQL的crash-safe原理解析](https://my.oschina.net/vivotech/blog/4289724/print)这篇讲了为什么不能只用redo log，易懂
- [MySQL是如何实现ACID中的D的](https://zhuanlan.zhihu.com/p/98778890)这篇讲了redo log, bin log 为什么要设计成二段提交，易懂
- [互联网项目中mysql应该选什么事务隔离级别](https://zhuanlan.zhihu.com/p/59061106)
- [三种日志的简单总结](https://www.cnblogs.com/wy123/p/8365234.html)
- [详解二段提交](https://juejin.im/post/6844904079215312909)
redo log， bin log这里网上来回抄，还一堆误导人的，稍微整了下：
- [我对redo log, bin log的总结](https://github.com/dabaitudiu/autumn_notes/blob/master/Database/rebin.md)
- [一条SQL语句执行得很慢的原因有哪些？](https://zhuanlan.zhihu.com/p/62941196)

### Redis
- redis一般考的不会太深，看个大概就够了，会redis是加分项
    1. [redis入门](https://www.nowcoder.com/courses/cover/live/473)
- [9. Redis Cluster](https://github.com/dabaitudiu/autumn_notes/blob/master/Redis/9.%20Redis_Cluster.md)

### 计算机网络
- 列的这些都是关键考点，不懂的看b站也行看知乎也行
- [经典问题：输入URL回车之后，究竟发生了什么](https://github.com/dabaitudiu/autumn_notes/blob/master/%E8%AE%A1%E7%AE%97%E6%9C%BA%E7%BD%91%E7%BB%9C/network1.md)
- [TCP三次握手，四次挥手](https://github.com/dabaitudiu/autumn_notes/blob/master/%E8%AE%A1%E7%AE%97%E6%9C%BA%E7%BD%91%E7%BB%9C/network2.md)
- [HTTP/HTTPS](https://github.com/dabaitudiu/autumn_notes/blob/master/%E8%AE%A1%E7%AE%97%E6%9C%BA%E7%BD%91%E7%BB%9C/network3.md)
- [TCP的可靠性保证](https://github.com/dabaitudiu/autumn_notes/blob/master/%E8%AE%A1%E7%AE%97%E6%9C%BA%E7%BD%91%E7%BB%9C/network4.md)
- [网络协议分层(暂缺)]()
- [Session、Cookie(暂缺)]()
- [TCP粘包、分包](https://github.com/dabaitudiu/autumn_notes/blob/master/%E8%AE%A1%E7%AE%97%E6%9C%BA%E7%BD%91%E7%BB%9C/network5.md)
