# OpenWRT for FriendlyElec NanoPi R4S

**本固件基于 [OpenWRT-21.02](https://github.com/openwrt/openwrt) 官方源码编译，默认使用 [Argon 主题](https://github.com/jerrykuku/luci-theme-argon)，固件内置一些常用插件。**

**固件下载（上游跟踪）：[https://github.com/sbwml/openwrt_build_r4s/releases](https://github.com/sbwml/openwrt_build_r4s/releases)**

默认参数
- IP地址：10.0.0.1
- 账户：root
- 密码：无

固件使用 nginx 作为默认web引擎，若要回退 uhttpd 请在终端执行以下操作：
- opkg update
- opkg install uhttpd uhttpd-mod-ubus
- /etc/init.d/nginx stop
- /etc/init.d/nginx disable
- /etc/init.d/uhttpd enable
- /etc/init.d/uhttpd start

**启用 IPv6 功能：登录后台 - 网络 - DHCP/DNS - 高级设置 - 过滤 IPv6 记录 （关闭） - 保存并应用**
