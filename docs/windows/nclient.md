> 该文档最后更新日期: 2019-03-27

<p class="info">我们不再支持本客户端，因为SS协议已被停用,您将无法创建新的LinkCode。</p>

### 介绍

NClient 是由NICO团队为Windows用户推出的一键客户端，您无需进行复杂的配置，只需创建一个唯一的LinkCode。

适用协议：`SS`

### 卸载

在部分版本的操作系统下，无法通过控制面板中卸载NClient。

您可以(Windows)+R 运行 `cmd.exe`，再输入 `MsiExec.exe /x {9C9746F8-D9D8-4A0B-AB1A-A3F19163C0B2}` 进行卸载。

### 下载

版本: 2.1.1 | 更新日期: 2017-12-22

[立即下载](https://dl.niconode.co/client/NClient-2.1.1-installer.exe)

### 权限与组件

- Windows XP 及 Vista 用户：
	- 请确保您的计算机安装了.NET Framework 2.0以及4.0，以免无法启动。
- Windows 7 及 以上用户：
	- 当您启用防火墙后，首次运行会显示将NClient及其组件拦截提示，请选择允许。
- 如果您安装了杀毒软件，请关闭或允许NClient的所有操作。

### 创建LinkCode

- 打开订阅中的`LinkCode`，点击磁贴进行创建。
	
![Tab](https://img.niconode.co/2017122114464923237uJ5qmAcjVMUYmAt.png)

- 输入一个用于辨识您计算机的命名，以及需要设置的线路节点。

	![选择](https://img.niconode.co/2017122114504295981PndmUvBEa8BsMCG.png)

- 一切就绪之后，您将得到一串随机生成的代码。

	![LinkCode](https://img.niconode.co/2017122114511496933z9v6sMweETFBMXM.png)

> LinkCode只会显示一次，<br/>
> 若意外丢失，您可以直接重新创建一个新的LinkCode，并移除旧的LinkCode。

<div class="danger">请勿将LinkCode以任何形式公布于网路中(包括但不限于论坛、聊天群组等)，以免您的流量消耗过快。</div>


### 启动NClient

完成安装后，打开桌面的 NClient，直接将刚才的LinkCode粘贴，选择`Quick Connect`。

> 当您在您客户端中使用后，会自动记住。 

### 自定义配置文件

NClient目前提供多种自定义选项。您只需要打开安装目录中，可修改`clients.conf`文件：

```
[common]
uuid = xxxxxxxx-18bc-11e7-8651-xxxxxxxxxxxx
//用于辨识您的机器，请不要清空，以免无法启动客户端。
bind = 127.0.0.1
//您的SOCKS5/HTTP代理绑定端口，修改成局域网/公网IP可分享给他人。SOCKS5端口：1068，HTTP代理端口：1078
alwaysproxy = true
//是否开启全局代理模式，改为false将只针对无法访问的站点（实验性功能）
debug = true
//记录日志，通常将记录您的有关错误。在不使用时，您可以设为false进行关闭。
[api]
linkcode = xxxxx
//用于记录您上次成功连接的LinkCode。
```

> 如果您运行NClient发生了闪退等错误，请您找到安装目录，将nclient.log反馈于我们
