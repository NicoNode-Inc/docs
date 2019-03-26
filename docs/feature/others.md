> 该文档最后更新日期: 2018-12-09

## UDP 转发

将DNS查询请求转发至我们的服务器，可配置于路由器、手机，有效的解析被污染的域名。

## TCP Fast Open

TCP 快速打开（英语：TCP Fast Open，简称TFO）是对计算机网络中传输控制协议（TCP）连接的一种简化握手手续的拓展，用于提高两端点间连接的打开速度。

需要 Linux 3.7+ 内核用户，Android用户需获取root权限，macOS 10.14/iOS12 开始支持该特性。

## AEAD

> 在通常的密码学应用中，Confidentiality（保密）用加密实现，消息认证用 MAC（Message Authentication Code，消息验证码）实现。这两种算法的配合方式，引发了很多安全漏洞，过去曾经有 3 种方法：
>
> Encrypt-and-MAC (E&M)
> MAC-then-Encrypt (MtE) <- 即 OTA 的做法
> Encrypt-then-MAC (EtM) <- 新协议的做法
> 然而后来人们发现，E&M 和 MtE 都是有安全问题的，所以 2008 年起， 逐渐提出了「用一个算法在内部同时实现加密和认证」的 idea，称为 AEAD (Authenticated Encryption with Associated Data)。在 AEAD 这种概念里，cipher + MAC 的模式被一个 AEAD 算法替换。

> 使用了 AEAD 算法的新协议本质上就是更完善的 stream cipher + authentication，虽然它依然使用的是流加密，但是通过更完善的数据包完整性验证机制杜绝了上面所述的可被篡改密文的可能性。

> 引用于[为何shadowsocks要弃用一次性验证(OTA)?](https://blessing.studio/why-do-shadowsocks-deprecate-ota/)

- 新的加密方式

|Name|Alias|
|---|---|
|AEAD_CHACHA20_POLY1305|chacha20-ietf-poly1305|
|AEAD_AES_256_GCM|aes-256-gcm|
|AEAD_AES_192_GCM|aes-192-gcm|
|AEAD_AES_128_GCM|aes-128-gcm|

## OBFS

<p class="tip">目前该特性已经停止支持</p>

![OBFS](https://img.niconode.co/2017022820450731639XCYQBvnKbeiUv3o.png)

- 介绍

如果您的设备支持，我们强烈建议您开启这个选项。

- 为什么要开启?

您的数据包将会被混淆，将对服务稳定性有小小提升。<br/>
以及，当您的网络被抓包时，将增大还原请求的难度。

部分地区ISP运营商以及三四级ISP运营商会根据数据包类型对您的数据包进行QoS，开启后也许会对您使用我们服务的稳定性得到小小改善。_未经验证_
