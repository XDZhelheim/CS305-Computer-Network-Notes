# 计算机网络 Computer Network

南方科技大学 计算机科学与工程系 11812804 董正

---

第一章 计算机网络概述
* 1.1 网络边缘 Network Edge
  * 1.1.1 接入网
    * 1.1.1.1 家庭接入 Home Network
    * 1.1.1.2 企业接入 Institutional Network (Ethernet)
    * 1.1.1.3 广域无线接入 Mobile Network
  * 1.1.2 物理媒体 Physical Media
* 1.2 网络核心 Network Core
  * 1.2.1 分组交换 Packet Switching
  * 1.2.2 电路交换 Circuit Switching
  * 1.2.3 因特网结构: 网络的网络
1.3 分组交换网中的时延、丢包和吞吐量
1.3.1 时延
1.3.2 排队时延和丢包
1.3.4 吞吐量 Throughput
1.4 协议层次 Protocol Layers
1.4.1 分层的体系结构
1.4.2 封装 Encapsulation
1.5 网络安全 Network Security
第二章 应用层 Application Layer
2.1 应用层协议原理 Principles of Network Applications
2.1.1 网络应用程序体系结构 Application Architectures
2.1.2 进程通信
2.1.3 可供应用程序使用的运输服务
2.1.4 因特网提供的运输服务
2.1.5 应用层协议 Application-layer Protocol
2.2 Web and HTTP
2.2.1 HTTP 概况
2.2.2 非持续连接和持续连接
2.2.3 HTTP 报文格式
2.2.4 Cookie
2.2.5 Web 缓存
2.2.6 条件 GET
2.3 电子邮件 E-Mail
2.3.1 电子邮件系统的组成
2.3.2 SMTP
2.3.3 邮件访问协议 Mail Access Protocol
2.4 DNS: 因特网的目录服务
2.4.1 DNS 提供的服务
2.4.2 DNS 的工作原理
2.4.2.1 分布式、层次数据库
2.4.2.2 DNS 缓存
2.4.3 DNS 记录和报文
2.5 P2P
2.5.1 P2P 体系结构的扩展性
2.5.2 BitTorrent
2.6 视频流与 CDN
2.6.1 因特网视频 Video Streaming
2.6.2 DASH
2.6.3 内容分发网 CDN
2.7 Socket 编程
第三章 运输层 Transport Layer
3.1 运输层服务 Transport Layer Services
3.2 多路复用与多路分解 Multiplexing & Demultiplexing
3.2.1 无连接的多路复用与多路分解
3.2.2 面向连接的多路复用与多路分解
3.3 UDP
3.3.1 UDP 的特性
3.3.2 UDP 检验和
3.4 可靠数据传输 Reliable Data Transfer
3.4.1 构造可靠数据传输协议
3.4.1.1 经完全可靠信道的可靠数据传输：rdt 1.0
3.4.1.2 经具有比特差错信道的可靠传输策略：rdt 2.0
3.4.1.3 rdt 2.1
3.4.1.4 rdt 2.2
3.4.1.5 经具有比特差错的丢包信道的可靠数据传输：rdt 3.0
3.4.2 流水线可靠数据传输协议
3.4.3 回退 N 步 Go-Back-N
3.4.4 选择重传 Selective Repeat
3.5 面向连接的运输: TCP
3.5.1 TCP 连接
3.5.2 TCP 报文段
3.5.3 TCP 序号和确认号
3.5.4 往返时间的估计与超时
3.5.5 可靠数据传输
3.5.6 流量控制 Flow Control
3.5.7 TCP 连接管理 Connection Management
3.6 拥塞控制原理 Principles of Congestion Control
3.6.1 情况 1：两个发送方和一台具有无限大缓存的路由器
3.6.2 情况 2：两个发送方和一台具有有限缓存的路由器
3.6.3 情况 3：4 个发送方和具有有限缓存的多台路由器和多跳路径
3.7 TCP 拥塞控制
3.7.1 慢启动 Slow Start
3.7.2 拥塞避免 Congestion Avoidance
3.7.3 快速恢复 Fast Recovery
3.7.4 TCP 吞吐量
3.7.5 TCP 公平性
3.7.6 明确拥塞通告：网络辅助拥塞控制
第四章 网络层: 数据平面 Network Layer: The Data Plane
4.1 网络层概述
4.1.1 转发和路由选择：数据平面和控制平面
4.1.2 网络服务模型 Network Service Model
4.2 路由器工作原理 Router
4.2.1 路由器结构概述 Router Architecture
4.2.2 输入端口处理和基于目的地转发
4.2.3 交换
4.2.4 输出端口处理
4.2.5 排队
4.2.6 分组调度
4.3 网际协议 Internet Protocol
4.3.1 IPv4 数据报格式
4.3.2 IPv4 数据报分片
4.3.3 IPv4 编址
4.3.4 网络地址转换 NAT
4.3.5 IPv6
4.4 通用转发和 SDN
第五章 网络层: 控制平面 Network Layer: The Control Plane
5.1 概述
5.2 路由选择算法 Routing Algorithm
5.2.1 链路状态路由选择算法 LS
5.2.2 距离路由向量算法 DV
5.3 因特网中自治系统内部的路由选择: OSPF
5.4 ISP 之间的路由选择: BGP
5.4.1 BGP 的作用
5.4.2 通告 BGP 路由信息
5.4.3 确定最好的路由
5.4.4 BGP 通告路由选择
5.4.5 Intra-AS 与 Inter-AS Routing 的比较
5.5 SDN 控制平面
5.5.1 SDN 结构
5.5.2 SDN 控制器
5.5.3 OpenFlow 协议
5.5.4 数据平面与控制平面交互的例子
5.6 ICMP: 因特网控制报文协议
5.7 网络管理和 SNMP
5.7.1 网络管理框架
5.7.2 简单网络管理协议 SNMP
第六章 链路层和局域网 Link Layer and LANs
6.1 链路层概述
6.1.1 链路层提供的服务
6.1.2 链路层在何处实现
6.2 差错检测和纠正技术 Error Detection and Correction
6.2.1 奇偶校验
6.2.2 循环冗余检测 Cyclic Redundancy Check
6.3 多路访问链路和协议 Multiple Access
6.3.1 信道划分协议 Channel Partitioning Protocol
6.3.2 随机接入协议 Random Access Protocol
6.3.2.1 时隙 ALOHA
6.3.2.2 ALOHA
6.3.2.3 载波侦听多路访问 CSMA
6.3.2.4 具有碰撞检测的 CSMA (CSMA/CD)
6.3.3 轮流协议 Taking-Turns Protocol
6.3.4 DOCSIS: 用于电缆因特网接入的链路层协议
6.4 交换局域网 LANs
6.4.1 链路层寻址和 ARP
6.4.2 以太网
6.4.3 链路层交换机
6.4.3.1 交换机转发和过滤
6.4.3.2 自学习 Self-Learning
6.4.3.3 链路层交换机的性质
6.4.3.4 交换机和路由器比较
6.4.4 虚拟局域网
6.5 链路虚拟化：网络作为链路层
6.6 数据中心网络 Data Center Networking
6.7 回顾：Web 页面请求的历程
6.7.1 准备：DHCP、UDP、IP 和以太网
6.7.2 仍在准备：DNS 和 ARP
6.7.3 还是在准备：域内路由选择到 DNS 服务器
6.7.4 Web 客户-服务器交互：TCP 和 HTTP
第七章 无线网络和移动网络 Wireless and Mobile Networks
7.1 概述
7.1.1 无线网络的组成
7.1.2 无线网络的分类
7.2 无线链路和网络特征
7.2.1 无线和有线的差别
7.2.2 信噪比和比特差错率
7.2.3 码分多址 CDMA
7.3 WiFi: 802.11 无线 LAN
7.3.1 802.11 体系结构
7.3.2 802.11 MAC 协议
7.3.3 IEEE 802.11 帧
7.3.4 在相同的 IP 子网中的移动性
7.3.5 802.11 中的高级特色
7.3.6 个人域网络：蓝牙和 ZigBee
7.4 蜂窝因特网接入 Cellular Internet Access
7.4.1 2G 蜂窝网体系结构：语音与电话网连接
7.4.2 3G 蜂窝数据网：将因特网扩展到蜂窝用户
7.4.3 走向 4G: LTE
7.5 移动管理原理
7.5.1 寻址
7.5.2 路由选择到移动节点
7.5.2.1 移动节点的间接路由选择 Indirect Routing
7.5.2.2 移动节点的直接路由选择 Direct Routing
