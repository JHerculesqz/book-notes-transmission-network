# L2 VPN的本质

* 类似二层交换机，记录了MAC地址表，一条路\(一个标签\)就有表中的一行记录

# L2 VPN的标签格式和标签变化流程

* STEP1.源PE添加隧道标签、VPN标签
* STEP2.源PE添加二层头部
  * 二层头部是下一跳Por宿PE的MAC地址
* STEP3.源PEorP根据二层头部向下一跳转发报文
* STEP4.Por宿PE收到报文后，更新报文的二层头部，更新为下一跳的MAC地址
* STEP5.宿PE收到报文后，解出VPN标签，将报文扔给对应的CE

![](/assets/Figure-0166-161.jpg)

# ![](/assets/Figure-0168-163.jpg)L2 VPN技术分类

* 点对点
* 点对多点
* 多点对多点

# L2 VPN的具体实现

* PWE3
* PWE3适合应用于点对点、点对多点



