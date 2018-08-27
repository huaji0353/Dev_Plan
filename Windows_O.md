## 一个极客应该有
修改版操作系统,加强网页浏览器,网络安全套件,软件安全套件,聊天娱乐,开发套件

## 项目总览
### 操作系统：

* [Windows10精简版](http://73376329.bokee.com/506177453.html)

### 网页浏览器(web browser)：

* Iridium/Ungoogled-Chromium ~~chrome 去谷歌化(谷歌套件)+隐私(强制https,去跟踪,cookie加强管理)与广告~~

### 浏览器增强插件：（Chromium有重定向冲突！)

* AdBlock(去广告)

* Header Editor(支持正则,强大的googleapi重定向/屏蔽)

* HTTPS Everywhere(对抗国内DPI)

### 网络安全：
#### DNS：Pcap_DNSProxy(对抗普通DNS污染,如FW原型开发出来,需整合)

#### DPI审查：goodbyedpi(对抗国内DPI,如FW原型开发出来,需整合)

#### 防火墙：基于WFP开发需求(windivert+winpcap+sqllite?)
* 端口识别(快速)/基础协议判断(tcp,udp,icmp/dns,http/dhcp,arp...) Will NOT support ipv6！(慢速,阻塞)

* Ban策略：IPBan(tcpip),HostBan(http) 支持非正则与正则设置选项

* 支持软件组策略,系统情景模式

* 标准wmi组件控制支持(以便ps脚本快速设置巨量规则)

### 软件安全：sandbox 基于minimalprocess + wine_win32(WinSer2008API 基本兼容)(开源Library os)

### 文本编辑器：notepad++/notepad2魔改

### 聊天娱乐：UWPqq|基于webqq/smartqq协议(二次开发很恶心,由于国内情况,只能兼容...)


## Windows10装机优化指南：（基于@73376329的w10企业精简版本 工具使用dism++)
### 基本优化
移除一堆微软自家的appx(去微软化)

### 网络隐私
关闭收集最近文件

### 软件安全
开启UAC

### 其他需求
TODO ...
