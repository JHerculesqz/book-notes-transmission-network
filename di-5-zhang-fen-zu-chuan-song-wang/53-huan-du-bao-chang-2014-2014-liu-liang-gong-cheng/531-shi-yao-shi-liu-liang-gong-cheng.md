# MPLS-TE与传统流量工程的区别

* 传统流量工程：指定N个隧道怎么走，好像交警交通管制说只能走光谷1路，不能走关山大道。这样可能导致光谷1路很堵，关山大道没有车。
* MPLS-TE：能控制N个隧道中每条业务怎么走。好像交警说张三的车走光谷1路、李四的车走关山大道、王五的车。。。。

# MPLS-TE的组成部件

* 信息发布部件：采集网络topo、带宽、负载

* 通路选择部件：算路。支持松散显示路由\(经过欢乐谷就行\)、严格显示路由（我要去中北路，走三环过严西湖隧道到欢乐谷）

* 信令部件：总控。协调、用一条路就减少总剩余资源。LDP、RSVP-TE
* 分组转发部件：路都算好了，按照安排执行就好。

![](/assets/Figure-0184-180.jpg)

