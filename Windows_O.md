### listedby @huaji0353


## 一个极客应该有
修改版操作系统,加强网页浏览器,网络安全套件,软件安全套件,聊天娱乐,开发套件


## 项目总览
### 操作系统：

* [Windows10精简版](http://73376329.bokee.com/506177453.html)

### 网页浏览器(web browser)：

* Iridium/Ungoogled-Chromium ~~chrome 去谷歌化(谷歌套件)+隐私(强制https,去跟踪,cookie加强管理)与广告~~

### 浏览器增强插件：（Chromium有重定向冲突！)

* violentmonkey([屏蔽SE的垃圾水站](https://greasyfork.org/scripts/1682-google-hit-hider-by-domain-search-filter-block-sites))

* AdBlock(去广告,保护隐私)

* Header Editor(支持正则,强大的googleapi与验证码重定向+屏蔽×FWblacklist)

* HTTPS Everywhere(对抗国内DPI)

### 网络安全：

#### DNS：Pcap_DNSProxy(对抗普通DNS污染,如FW原型开发出来,需整合)

#### DPI审查：(已证明无效,反而被监视注意) ~~goodbyedpi(对抗国内DPI,如FW原型开发出来,需整合)~~

#### 防火墙：基于WFP开发需求(windivert+winpcap+sqllite?)
* 端口识别(快速)/基础协议判断(tcp,udp,icmp/dns,http/dhcp,arp...) I Will NOT support ipv6！(慢速,阻塞)

* Ban策略：IPBan(tcpip),HostBan(http) 支持非正则与正则设置选项

* 支持软件组策略,系统情景模式

* 标准wmi组件控制支持(以便ps脚本快速设置巨量规则)

### 软件安全：
#### sandbox 基于minimalprocess + wine_win32(WinServ2008API 基本兼容)(开源Library os)

### 文本编辑器：
#### notepad++/notepad2魔改

### 聊天娱乐：
#### UWPqq or 基于webqq/smartqq协议(二次开发很恶心,由于国内情况,只能兼容...)


## Windows10基本装机指南：（基于@73376329的w10企业精简版本)

### 基本优化
移除一堆微软自家的appx(去微软化 工具使用dism++)

### 网络隐私
关闭收集最近文件

安装第三方开源防火墙

开启httpsoverdns

### 软件安全
开启UAC

安装沙盒(如是Serv2016,Windows docker/Container了解一下)

### 其他需求
TODO ...
