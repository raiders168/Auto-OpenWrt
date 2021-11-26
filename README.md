# 云编译 OpenWrt 固件

## 项目说明

**增强项**：（**打勾项**默认**编译**入固件；**未打勾项**默认**不编译**入固件。）
  - [x] 架构适配x86_64
   - [x]后台地址：192.168.1.1 管理员：root  初始密码：空
  - [x] 添加jerrykuku第三方argon主题 并设置为默认
  - [x] 添加科学上网插件 passwall
  - [x] 添加DNS加强插件  smartdns
  
**精简项**：
  - [x] luci-app-accesscontrol
  - [x] luci-app-adbyby-plus
  - [x] luci-app-arpbind
  - [x] luci-app-ddns
  - [x] luci-app-ipsec-vpnd
  - [x] luci-app-rclone
  - [x] luci-app-upnp
  - [x] luci-app-uugamebooster
  - [x] luci-app-vsftpd
  - [x] luci-app-xlnetacc
  - [x] luci-app-zerotier

![N1_OpenWRT.png](https://i.loli.net/2021/08/27/u4318mKdQlYtek2.png)

## 感谢 ❤️
- 源码来源： Lean 的 Openwrt 源码仓库 https://github.com/coolsnowwolf/lede
- 脚本来源： P3TERX 的 使用 GitHub Actions 云编译 OpenWrt https://github.com/P3TERX/Actions-OpenWrt
