# OpenWRT for FriendlyElec NanoPi R4S

**本固件基于 [OpenWRT-21.02](https://github.com/openwrt/openwrt) 官方源码编译，默认使用 [Argon 主题](https://github.com/jerrykuku/luci-theme-argon)，固件内置一些常用插件。**

**固件下载：[OpenWRT-NanoPi_R4S](https://media.cooluc.com/%E6%96%87%E4%BB%B6/OpenWRT-NanoPi_R4S)**

默认信息：
- IP地址：10.0.0.1
- 账户：root
- 密码：无

AdGuard Home：

- 账户：root
- 密码：password

固件使用 nginx 作为默认web引擎，若要回退 uhttpd 请在终端执行以下操作：
- opkg update
- opkg install uhttpd uhttpd-mod-ubus
- /etc/init.d/nginx stop
- /etc/init.d/nginx disable
- /etc/init.d/uhttpd enable
- /etc/init.d/uhttpd start

## 固件演示

**演示地址：[http://openwrt.cooluc.com/](http://106.55.142.145:8888/)**

**账户：root**

**密码：无**
