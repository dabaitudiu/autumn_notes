# autumn_notes
preparations and notes

#### 操作系统
[进程相关问题1](https://github.com/dabaitudiu/autumn_notes/blob/master/Operating%20System/7.%20%E8%BF%9B%E7%A8%8B%E4%B8%8E%E7%BA%BF%E7%A8%8B.md) &nbsp; &nbsp;[Source Video](https://www.bilibili.com/video/BV1js411b7vg?p=42)

#### JVM
[问题集](https://github.com/dabaitudiu/autumn_notes/blob/master/JVM/%E9%97%AE%E9%A2%98%E9%9B%86.md)

#### 多线程
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

#### 数据库
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
<br>
唉。日志这块，看来看去，他抄他，他抄他，乱的不行，看吐了都。说一下我的理解和总结：


#### 首先为什么有bin log:
- 这是MySQL Server本身提供的一个恢复机制，能让你通过依次执行bin log的SQL语句达到某一个时间节点的数据。
- 另外，MySQl也是通过bin log实现主从复制的，设计了一个bin log dump 线程来完成这个过程，这个是MySQL自带的，没有为什么，就是这么设计的。
- 但是这个设计存在un-crash-safe的问题，比如主从复制时，bin log已经传给了slave节点，slave执行后具有了数据。但是master节点在写入磁盘的时候宕机了，数据没能写入，这个时候就出现了主从不一致的问题。
- 第二种情况：假设即使是单机的环境，有一个事务有2条语句，第一条已经提交成功了，binlog也写完了，第二条只是binlog写了，整个事务没有提交。这时候如果宕机，重启后第一条binlog，系统会认为已经完成了commit, 所以不会重新执行binlog，尽管第二天binlog，系统会回滚然后重新执行语句，但是binlog1的数据已经丢失，所以不是crash-safe。

#### crash-safe
所以InnoDB在引擎层面引入了redo-log来实现crash-safe特性。如何实现crash-safe, WAL(write-ahead logging)机制：
```
    Imagine a program that is in the middle of performing some operation when the machine it is 
    running on loses power. Upon restart, that program might need to know whether the operation 
    it was performing succeeded, succeeded partially, or failed. If a write-ahead log is used, 
    the program can check this log and compare what it was supposed to be doing when it unexpectedly 
    lost power to what was actually done.
```

#### redo log
redo log的属性: 
```
内容：物理格式的日志，记录的是物理数据页面的修改的信息，其redo log是顺序写入redo log file的物理文件中去的。
什么时候产生：事务开始之后就产生redo log，redo log的落盘并不是随着事务的提交才写入的，而是在事务的执行过程中，便开始写入redo log文件中.
```
所以可见redo log实现了这个WAL特性，也实现了crash-safe。 把 redo log 写到磁盘，比一般的写磁盘要快，原因有：一般我们写磁盘，都是「随机写」，而 redo log，是「顺序写」；MySQL 在写 redo log 上做了优化，比如「组提交」

#### 能不能只用redo-log? 
不能。redo log 是循环写，写到末尾是要回到开头继续写的。这样历史日志没法保留，redo log 也就起不到归档的作用。再有一个重要原因是之前提到的MySQL利用bin log做主从复制，这个没法从引擎层面上改

#### 不使用二段提交的问题:
是先写完redo log 还是先写完bin log？还是穿插？
1. 先写 redo log，再写 binlog。这样会出现 redo log 写入到磁盘了，但 binlog 还没写入磁盘，于是当发生 crash recovery 时，恢复后，主库会应用 redo log，恢复数据，但是由于没有 binlog，从库就不会同步这些数据，主库比从库“新”，造成主从不一致 
2. 先写 binlog，再写 redo log，跟上一种情况类似，很容易知道，这样会反过来，造成从库比主库“新”，也会造成主从不一致。

#### 那为啥二段提交就能避免？
时间点1 -> prepare阶段 -> 时间点2 -> commit阶段 -> 时间点3

    时间点1出现问题:
    这个时候redo log 和 binlog都在内存中，所以本次事务的相关操作都会消失，相对于事务回滚了，不影响数据的一致性。

    时间点2出现问题:
    这个时候redo log已经到磁盘了。binlog没有刷到磁盘所以会消失。服务器从故障中恢复时，读取磁盘中的redo log ，
    但是由于对应的redo log项还是prepare状态，就要判断binlog 是否完整，如果binlog完整则提交事务，如果binlog不完整则回滚事务。

    时间点3出现问题。:
    这个时候redo log 和 binlog都已经存磁盘，服务器从redo log恢复就好了。

##### binlog怎么判断完整性
    - statement 格式的 binlog，最后会有 COMMIT；
    - row 格式的 binlog，最后会有一个 XID event
