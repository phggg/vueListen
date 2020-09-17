## HTTP请求｜HTTP的协议解析

### TCP与IP的一些基础知识

- 流
- 端口
- require('net')
- 
- 包
- IP地址
- libnet/libpacp

1. TCP层传输数据的概念是流，没有明显的分割单位，只保证前后顺序正确， TCP对应一个重要的概念叫端口，计算机的网卡根据端口把接到的数据包分给各个应用，对用node中的net包
2. IP传输的概念是一个一个数据包的概念，IP根据地址找到包在哪里
3. libnet和libpacp是C++的两个库，libnet负责构造ip包并发送，libpacp负责抓所有流经网卡的IP包

**TCP/IP是全双工通道，可以互相发送 **

### HTTP

**HTTP是由request和response这样的过程组成的，HTTP必须先由客户端发起一个request，然后服务端返回一个response，每一个request必须对应唯一一个response**

