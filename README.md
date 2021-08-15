<center><img src="https://upload.wikimedia.org/wikipedia/commons/8/84/OpenWrt_Logo.svg" width="380px" alt="openwrt" /></center>

<center><h1>OpenWRT for FriendlyElec NanoPi R4S</h1></center>

**本固件基于 [OpenWRT-21.02](https://github.com/openwrt/openwrt) 官方源码编译，默认使用 [Argon 主题](https://github.com/jerrykuku/luci-theme-argon)，固件内置一些常用插件。**

**固件下载：[OpenWRT-NanoPi_R4S](https://media.cooluc.com/%E6%96%87%E4%BB%B6/OpenWRT-NanoPi_R4S)**

### 默认信息

- **管理地址：http://10.0.0.1 或 http://openwrt.lan**
- **账户：root**
- **密码：无**

**AdGuard Home：**

- **账户：root**
- **密码：password**

**固件使用 nginx 作为默认web引擎，若要回退 uhttpd 请在终端执行以下操作：**
```shell
opkg update

opkg install uhttpd uhttpd-mod-ubus

/etc/init.d/nginx stop

/etc/init.d/nginx disable

/etc/init.d/uhttpd enable

/etc/init.d/uhttpd start
```

### 固件演示

**演示地址：**[http://openwrt.cooluc.com/](http://106.55.142.145:8888/)

**账户：root**

**密码：无**

### 固件区分

**固件分为两个文件系统，[SquashFS](https://zh.wikipedia.org/wiki/SquashFS) 和 [Ext4](https://zh.wikipedia.org/wiki/Ext4)。**

**SquashFS（推荐）：SquashFS 为只读文件系统，支持系统还原（支持物理 Reset按钮 还原），支持后台固件升级，更能避免 SD 卡文件系统触发写保护，适合绝大部分用户使用。**

**Ext4：Ext4 文件系统具备整个分区可读写性质，更适合熟悉 Linux 系统的用户使用。**


### 插件列表

<details>
    <summary>展开查看</summary>
<pre>
CPU 性能调节设置
Docker
USB 打印服务器
应用过滤（需要关闭 “防火墙 - FullCone-NAT 和 软件流量分载”）
PassWall
文件浏览器
AdGuard_Home
ShadowSocksR_Plus+
微信推送
OpenClash
解除网易云音乐播放限制
动态 DNS
硬盘休眠
带宽监控
KMS 服务器
网络共享
Transmission
Aria2
迅雷快鸟
frp 服务器
frp 客户端
终端
UPnP
SmartDNS
ZeroTier
</pre>
</details>
