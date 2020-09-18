# autumn_notes
preparations and notes

### 操作系统
[进程相关问题1](https://github.com/dabaitudiu/autumn_notes/blob/master/Operating%20System/7.%20%E8%BF%9B%E7%A8%8B%E4%B8%8E%E7%BA%BF%E7%A8%8B.md) &nbsp; &nbsp;[Source Video](https://www.bilibili.com/video/BV1js411b7vg?p=42)

### JVM
[问题集](https://github.com/dabaitudiu/autumn_notes/blob/master/JVM/%E9%97%AE%E9%A2%98%E9%9B%86.md)

### 多线程
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

### Redis
- [9. Redis Cluster](https://github.com/dabaitudiu/autumn_notes/blob/master/Redis/9.%20Redis_Cluster.md)

### 计算机网络
- [经典问题：输入URL回车之后，究竟发生了什么](https://github.com/dabaitudiu/autumn_notes/blob/master/%E8%AE%A1%E7%AE%97%E6%9C%BA%E7%BD%91%E7%BB%9C/network1.md)
- [TCP三次握手，四次挥手](https://github.com/dabaitudiu/autumn_notes/blob/master/%E8%AE%A1%E7%AE%97%E6%9C%BA%E7%BD%91%E7%BB%9C/network2.md)
- [HTTP/HTTPS](https://github.com/dabaitudiu/autumn_notes/blob/master/%E8%AE%A1%E7%AE%97%E6%9C%BA%E7%BD%91%E7%BB%9C/network3.md)
