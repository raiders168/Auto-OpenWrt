# 云编译 OpenWrt 固件

**项目说明**：
- 本项目使用 Github Actions 下载 [Lean](https://github.com/coolsnowwolf/lede) 的 `Openwrt` 源码仓库，进行云编译。
- 本项目使用定时编译（北京时间每周日下午4点开始自动运行编译）及触发编译（更新script.sh后可开始编译）两种方式。
- 本项目同时编译5.4内核、5.10内核、5.15内核、6.1内核固件
- 本项目编译固件适配 X86_64架构
- 本项目编译固件后台地址：192.168.1.2 管理员：root  初始密码：空
- 本项目相对源码默认设置做了如下更改：

**特色插件**：
  - [x] 添加 jerrykuku第三方argon主题 并设置为默认
  - [x] 添加 jerrykuku第三方argon主题 管理设置
  - [x] 添加科学上网插件 passwall
  - [x] 添加本地DNS服务器插件 smartdns
  
**集成插件**：（**打勾项**默认**编译**入固件、**未打勾项**默认**不编译**入固件）
  - [x] luci-app-accesscontrol  #访问时间控制
  - [x] luci-app-adbyby-plus  #广告屏蔽大师Plus +
  - [x] luci-app-arpbind  #IP/MAC绑定
  - [x] luci-app-autoreboot  #支持计划重启
  - [x] luci-app-aliyundrive-webdav  #阿里云盘WebDAV
  - [x] luci-app-ddns   #动态域名 DNS（集成阿里DDNS客户端）
  - [x] luci-app-diskman   #磁盘管理工具
  - [x] luci-app-filetransfer  #文件传输（可web安装ipk包）
  - [x] luci-app-firewall   #添加防火墙
  - [x] luci-app-frpc   #内网穿透Frp客户端
  - [x] luci-app-frps   #内网穿透Frp服务端
  - [x] luci-app-hd-idle  #硬盘休眠
  - [x] luci-app-ipsec-vpnd  #VPN服务器 IPSec
  - [x] luci-app-mwan3   #MWAN3负载均衡
  - [x] luci-app-mwan3helper   #MWAN3分流助手
  - [x] luci-app-netdata  #Netdata实时监控（图形化）
  - [x] luci-app-nlbwmon   #网络带宽监视器
  - [x] luci-app-openvpn   # VPN客户端
  - [x] luci-app-openvpn server  # VPN服务器
  - [x] luci-app-passwall  #科学上网（Li大内插件）
  - [x] luci-app-ramfree  #释放内存
  - [x] luci-app-samba   #网络共享（Samba）
  - [x] luci-app-smartdns  #SmartDNS本地服务器
  - [x] luci-app-softethervpn  #SoftEther VPN服务器  NAT穿透
  - [x] luci-app-syncdial  #多拨虚拟网卡（原macvlan）
  - [x] luci-app-ttyd   #网页终端命令行
  - [x] luci-app-turboacc   #Turbo ACC 网络加速(支持 Fast Path 或者 硬件 NAT) 
  - [x] luci-app-unblockmusic  #解锁网易云灰色歌曲
  - [x] luci-app-upnp   #通用即插即用UPnP（端口自动转发）
  - [x] luci-app-usb-printer  #USB 打印服务器
  - [x] luci-app-vlmcsd  #KMS服务器设置
  - [x] luci-app-vsftpd  #FTP服务器
  - [x] luci-app-wireguard  #VPN服务器
  - [x] luci-app-wol   #WOL网络唤醒
  - [x] luci-app-zerotier  #ZeroTier内网穿透

**系统截图**：

<img width="805" alt="openwrt" src="https://user-images.githubusercontent.com/59355325/143574001-02a80f54-a188-460e-83d1-6f08428ba57e.png">

## 感谢 ❤️
- 源码来源： Lean 的 Openwrt 源码仓库 https://github.com/coolsnowwolf/lede
- 脚本来源： P3TERX 的 使用 GitHub Actions 云编译 OpenWrt https://github.com/P3TERX/Actions-OpenWrt
- 更新讨论群：[点击加入"OpenWRT+PassWall+SmartDNS（固件）讨论群](https://t.me/Raiders_openwrt)

