**English** | [中文](https://p3terx.com/archives/build-openwrt-with-github-actions.html)

# 云编译 OpenWrt 固件

云编译 OpenWrt 固件


## 项目说明

- 说明：

本项目使用 Github Actions 下载 Lean 的 Openwrt 源码仓库，进行云编译。
本项目使用定时编译（北京时间每周日下午4点开始自动运行编译）及触发编译（更新script.sh后可开始编译）两种方式。
本项目编译固件适配斐讯 N1 盒子，如需刷机，另需使用打包工具生成刷机固件。
本项目相对源码默认设置做了如下更改：
增强项：（打勾项默认编译入固件；未打勾项默认不编译入固件。）

 修改架构适配斐讯 N1 盒子
 添加 Perl依赖
 修改登录IP为 192.168.2.2，网关、DNS为 192.168.2.1，关闭DHCP服务
 添加主题 opentomacat 并设置为默认
 添加第三方插件 luci-app-openclash
 添加无线功能（待测试）
 启用 Docker （系统——启动项：启动）
 添加第三方插件 luci-app-vssr
精简项：

 luci-app-accesscontrol
 luci-app-adbyby-plus
 luci-app-arpbind
 luci-app-ddns
 luci-app-ipsec-vpnd
 luci-app-rclone
 luci-app-upnp
 luci-app-uugamebooster
 luci-app-vsftpd
 luci-app-xlnetacc
 luci-app-zerotier



## Tips

- 

## Credits

- [Microsoft Azure](https://azure.microsoft.com)
- [GitHub Actions](https://github.com/features/actions)
- [OpenWrt](https://github.com/openwrt/openwrt)
- [Lean's OpenWrt](https://github.com/coolsnowwolf/lede)
- [tmate](https://github.com/tmate-io/tmate)
- [mxschmitt/action-tmate](https://github.com/mxschmitt/action-tmate)
- [csexton/debugger-action](https://github.com/csexton/debugger-action)
- [Cowtransfer](https://cowtransfer.com)
- [WeTransfer](https://wetransfer.com/)
- [Mikubill/transfer](https://github.com/Mikubill/transfer)
- [softprops/action-gh-release](https://github.com/softprops/action-gh-release)
- [ActionsRML/delete-workflow-runs](https://github.com/ActionsRML/delete-workflow-runs)
- [dev-drprasad/delete-older-releases](https://github.com/dev-drprasad/delete-older-releases)
- [peter-evans/repository-dispatch](https://github.com/peter-evans/repository-dispatch)

## License

[MIT](https://github.com/P3TERX/Actions-OpenWrt/blob/main/LICENSE) © [**P3TERX**](https://p3terx.com)
