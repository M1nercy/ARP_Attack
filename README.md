# ARP-
基于Libpcap、Libnet的ARP攻击cpp代码
基于Libnet和Libpcap的ARP攻击程序，环境为Debian Linux，图形界面使用QT5开发 学生练手使用，操作逻辑上还有许多问题，能用就行 左下角的框框里先点抓包再点嗅探，可以嗅探指定IP的MAC地址（如果存货），获得想要的MAC地址后建议关闭抓包。右边的框框中： 选择定向攻击，发送的目标为目的IP、目的MAC对应的主机，目的IP和MAC地址需为真实地址，源IP和MAC可以自己随便写，但是要是局域网中存活的主机 选择广播攻击，发送的数据包为Gratuitous ARP数据包，此时目的IP和MAC就没用了，但是不可以为空（问就是懒得修BUG改UI），随便填一个符合地址格式的数字就行，发包进行不会理会该字符串。

需要安装的库为Libpcap和Libnet，可以自己搜索安装。
