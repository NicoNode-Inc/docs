> 该文档最后更新日期: 2018-06-07

<p class="info">我们对本客户端提供「一般」支持</p>

## 简介

Shadowsocks for Android 是一个有社区开发者支持并维护的客户端，目前已被收录于Shadowsocks官方项目中。

<p class="tip">如果您在使用中遇到任何问题，请前往社区发起Issue。[前往](https://github.com/shadowsocks/shadowsocks-android/issues)</p>

## 下载

根据您的操作平台，选择不同的版本将会达到更好的性能。

版本号：4.5.7 | 更新日期: 2018-4-24

- 通用版

[立即下载](https://dl.niconode.co/client/shadowsocks--universal-4.5.7.apk) | [Github下载](https://github.com/shadowsocks/shadowsocks-android/releases/download/v4.5.7/shadowsocks--universal-4.5.7.apk)

- ARM 64

[立即下载](https://dl.niconode.co/client/shadowsocks-arm64-v8a-4.5.7.apk) | [Github下载](https://github.com/shadowsocks/shadowsocks-android/releases/download/v4.5.7/shadowsocks-arm64-v8a-4.5.7.apk)

- ARM Eabi

[立即下载](https://dl.niconode.co/client/shadowsocks-armeabi-v7a-4.5.7.apk) | [Github下载](https://github.com/shadowsocks/shadowsocks-android/releases/download/v4.5.7/shadowsocks-armeabi-v7a-4.5.7.apk)

- x86

[立即下载](https://dl.niconode.co/client/shadowsocks-x86-4.5.7.apk) | [Github下载](https://github.com/shadowsocks/shadowsocks-android/releases/download/v4.5.7/shadowsocks-x86-4.5.7.apk)

## OBFS混淆

> 如果您开启了这个选项，您需要在手机上安装这个客户端。

#### 简介
OBFS是一个新特性，可以通过获取您设置的域名的页面内容，用以混淆数据包。[详细](/feature/others?id=obfs)

#### 下载

版本号：0.0.5 | 更新日期: 2017-02-15

[立即下载](https://dl.niconode.co/client/obfs-local-nightly-0.0.5.apk) | [Github下载](https://github.com/shadowsocks/simple-obfs-android/releases/download/v0.0.5/obfs-local-nightly-0.0.5.apk)

## 快速设置

- 打开我的订阅，在您要添加的线路最右侧。

	![](https://img.niconode.co/20180607131846753022wGBpcsjD5HQZt0.png)

- 点击链接按钮后，将会唤醒您的客户端。

	![](https://img.niconode.co/2016061520152049836Xqr3W1kMaVBOHXt.jpg)

- 选择`确定`后，您的客户端将会多出可用的线路。

- 您可以重复该操作以添加多个不同的线路。

## 二维码设置

- 您可以点击`二维码按钮`，您的其他手机/朋友可以直接通过该应用扫描添加。

## 开始连接

- 选择右下角的纸飞机按钮，以连接服务。

	![](https://img.niconode.co/2017072404094460187mtA4Q105YqBAgIO.png)

## 后台锁定策略

Shadowsocks将会调用系统的VPN接口与App进行数据交互，在部分定制化系统（包括但不限于Samsung Experience、MIUI）中，系统将会不定期的对后台进程进行清理。

我们建议您手动将 Shadowsocks 加入白名单中。

### Samsung Experian 9.0

- 点击右上角的选项菜单，选择`锁定应用程式`。

![](https://img.niconode.co/2018060813400552811NC1X3BEE8v7DCpI.jpg)

- 锁定后，点击完成。

- 打开`系统设置`--`设备维护`--`电池`--`未监控的应用程序`，手动添加`Shadowsocks`。

![](https://img.niconode.co/20180608134130825189RFUoYOQi9ECr42.jpg)

### MIUI 9.0

- 打开后台进程管理

- 按住Shadowsocks程序往下拉。

![](https://img.niconode.co/2018060813424349869C16XPuu3EhTlJSu.jpg)

- 点击上锁。

![](https://img.niconode.co/2018060813431591887UvqaOqDMrvYEJjt.jpg)
