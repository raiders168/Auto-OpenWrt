**English** | [中文](https://p3terx.com/archives/build-openwrt-with-github-actions.html)

# 云编译 OpenWrt 固件

## 项目说明

**增强项**：（**打勾项**默认**编译**入固件；**未打勾项**默认**不编译**入固件。）
  - [x] 修改架构适配斐讯 N1 盒子
  - [x] 添加 Perl依赖
  - [x] 修改登录IP为 192.168.2.2，网关、DNS为 192.168.2.1，关闭DHCP服务
  - [x] 添加主题 opentomacat 并设置为默认
  - [x] 添加第三方插件 luci-app-openclash
  - [x] 添加无线功能（待测试）
  - [x] 启用 Docker （系统——启动项：启动）
  - [x] 添加第三方插件 luci-app-vssr

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
