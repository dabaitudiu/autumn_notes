# 二、TCP三次握手，四次挥手
备考请看参考:[TCP/IP、三次握手四次挥手过程](https://zhuanlan.zhihu.com/p/103000747)， 本文只用于个人复习用

## 三次握手
1. 握手指的是：一次数据包发送和接收的过程
2. 我们假设客户端向服务端发起连接。
    - client会向server发送一个报文段，在报文段中，有一系列状态码，把SYN为置成1，代表想要发起连接。同时报文段中的序号设置成client_isn. server端收到后，会为收到的报文段分配TCP缓存和变量（泛洪攻击的原因），第一次握手完成
    - server准备向client发送一个报文段。在报文段中，把状态码SYN设置成1，ACK设置成1， 序号设置成server_isn, 确认号设置成client_isn + 1, 发出报文段。client收到后，第二次握手完成
    - client向server发送一个报文段，SYN = 0, ACK = 1，确认号 = server_isn + 1, 序号 = client_isn + 1。第三次握手完成
### 为什么要三次握手，不是两次
这个网上争议还是挺大的[TCP 为什么三次握手而不是两次握手（正解版）](https://blog.csdn.net/lengxiao1993/article/details/82771768)
我如果答的话：
第二次握手时，server向client发送了报文段，此时server就默认连接已经建立，然而如果报文段没能成功到达client，client就会等待一段时间重新发送连接请求。而server可能已经开始发送数据包了，接收到后来的连接请求也会拒绝，无法建立起连接。此外，对于一个无法建立的连接，服务器还是会为其分配资源，造成资源浪费，所以不能只用两次握手。（多了记不住）

### 为什么要client_isn, server_isn
在互联网不可靠通信的基础上，只有收到对方的回复，才能确保对方收到了你发送的序列号。所以一发一收，可以告知对方你选择的序列号起点，双方都各自选了一个序列号起点需要被对方知道。
第二次握手，服务器发出的seq ，客户端没收到, 此时连接就算建立的话 服务器此时主动发一个 seq = 123 的数据包过去， 客户端也不能知道这个请求是哪个TCP连接的第几个数据包吗 （一个客户端和一个服务器端的TCP链接是可以建立多个的）

###  客户端正在和服务端建立 TCP 连接，然而当服务器变 SYN-RCVD 后，此时一个旧的 SYN 报文 又到达了，服务器会如何处理
服务端在SYN_RECEIVED状态下，接收到旧的SYN 报文时是不能作出判断的，而是照常返回，当客户端接收到该报文后发现异常，才会发送RST 报文，重置连接。

### 知道SYN攻击吗？如何防范？
1. 第一次握手后，server会为tcp连接分配缓存，存放在半连接队列中。如果黑客伪造大量ip，向server发起连接请求，server会不断分配缓存，同时不断向这些ip发送连接请求而得不到回复，尝试多次后才会断开连接。这个过程中会造成服务器资源耗尽。
2. 解决方法：syn cookie. 第一次握手后不为client分配缓存，只有当client返回的ack报文段ack = server_isn + 1时，才展开全连接
3. syn cookie的问题: 由于没有半连接队列，server失去了重传SYNACK报文段的能力，假设server一直没收到client发来的ACK报文段，它可以认为client是黑客伪造的ip，就不会重传。然而，实际情况可能是SYNACK报文传递过程中丢失。

## 四次挥手
首先四次挥手比三次握手多了一次的原因，是因为当client向server发送断开连接的请求时，server有可能还没准备好，需要准备时间才能返回。具体流程如下：
1. client->server，FIN = 1， seq = client_isn + 1, client: FIN-WAIT-1
2. server->client, FIN = 0, ACK = 1, ack = client_isn + 1, ”知道了，准备好告诉你“, server: CLOSE-WAIT
3. server->client, FIN = 1, ACK = 1, ack = client_isn + 1, seq = server_isn, server: LAST-ACK
4. client->server, FIN = 0, ACK = 1, ack = server_isn + 1, seq = client_isn + 1, client: TIME-WAIT, 等待可能出现的要求重传的ACK报文. 两个最大段生命周期后，没有收到server的ACK报文，认为服务器端已经正常关闭连接，于是自己也关闭连接，进入 CLOSED 状态。

### 为什么不是5次
最后一次，server都关了，不能再发ack了。此外，4次已经足够了。

### 为什么需要TIME-WAIT状态
要确保服务器是否已经收到了我们的ACK 报文，如果没有收到的话，服务器会重新发FIN 报文给客户端，那么客户端再次收到FIN 报文之后，就知道之前的 ACK 报文丢失了，就会再次发送ACK 报文。

### 为什么 TIME_WAIT 状态需要经过 2MSL 才能转换到 CLOSE 状态
以LAST ACK的server的角度: 发送 + client ack确认，总共2MSL时间。如果这段时间没返回，就重发。重发的信息又会占用1MSL的时间。所以，站在client的角度：发送ACK，server没收到，占用1MSL, 等待server的重发请求，又要1MSL时间。如果这么长时间没收到，就说明断开连接请求已被确认。

