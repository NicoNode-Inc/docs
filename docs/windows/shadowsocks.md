> 该文档最后更新日期: 2019-03-27

<p class="info">我们对本客户端提供「一般」支持</p>

### 介绍

Shadowsocks C# 是一个开源的客户端。

适用协议：`SS`

### 下载

版本: 4.0.10 | 更新日期: 2018-05-11

[立即下载](https://dl.niconode.co/client/Shadowsocks-4.0.10.zip) | [GitHub下载](https://github.com/shadowsocks/shadowsocks-windows/releases/download/4.0.10/Shadowsocks-4.0.10.zip)

### 快速导入

- 先运行一次`Shadowsocks.exe`，然后退出。

- 选择订阅中的`客户端订阅`，选择以`(API v1.2)`开始的行列中，最右侧的`下载配置文件`。

	![快速添加](https://img.niconode.co/2019032708335041052c9auReqSdObI8bS.png)

- 您的浏览器将会下载一个`gui-config.json`，覆盖至`Shadowsocks.exe`的所在目录。

- 重新打开客户端，所有服务器已被自动添加。

### 手动添加

- 选择订阅中的`订阅列表`，找到需要添加的线路，选择`获取详细的连接信息`

	![](https://img.niconode.co/2018060611554434584wrF66J5RHF8UoNe.png)

- 显示详细的连接信息，不要关闭窗口。

	![](https://img.niconode.co/2018060611571968548TXCuSHrEukKM66U.png)

- 选择托盘中的 ![客户端图报表](https://img.niconode.co/2016071616450811168tAtlZ3XAa4JOkSm.png)，右键选择`服务器`中的`编辑服务器`。

	![](https://img.niconode.co/2018060611540081861NdPFj2OyNgLjb43.jpg)

- 依次将`服务器地址`，`服务器端口`，`密码`，`加密方式`，填入。

	- 如果您开启了OBFS，在`插件程序`填写`obfs-local`。
	- 如果您选择了HTTP混淆，在`插件选项`，第一个分号内容填写`obfs=http;`
	- 如果您选择了TLS混淆，在`插件选项`，第一个分号内容填写`obfs=tls;`
	- 接着上一条的分号，继续填写`obfs-host=域名`，例如`obfs-host=cloudflare.com`。
	- 例如您开启了OBFS，并且是TLS混淆，那么您的`插件选项`则应该是`obfs=tls;obfs-host=cloudflare.com`。

- 添加完成了后，您就可以使用我们的服务了。

### Chrome 浏览器拓展设置

> 您需要现在下载这个拓展，[点击下载](https://dl.niconode.co/extensions/SwitchyOmega.crx) 或 [GitHub下载](https://github.com/FelisCatus/SwitchyOmega/releases/download/v2.3.21/SwitchyOmega.crx)

- 开启开发者模式

- 在您的 Chrome 浏览器中访问 `chrome://extensions/`
	
	![img](https://img.niconode.co/2017022623273770747VNtwGa8iM3BLEj5.png)

- 勾选`开发者模式`

- 安装拓展

- 将刚才下载的`SwitchyOmega.crx`，直接拖动至浏览器窗口。

	![alert](https://img.niconode.co/20170226232840445234N9g1XiHYxUBb4O.png)

- 选择`添加拓展程序`

#### 配置全局模式

- 打开拓展程序首选项，通常来说您的本地端口是`1080`。

- 如下配置默认的情景模式。

	![proxy](https://img.niconode.co/2017022623302525929gbGZc4ylFHjfIJN.png)

- 保存，这个时候您可以使用Chrome中的全局代理功能了。

#### 配置智能模式

- 根据下载进行设置：
	1. 选择`添加规则`。
	2. 在`规则列表列表`中填写`https://raw.githubusercontent.com/gfwlist/gfwlist/master/gfwlist.txt`。
	3. 在`切换规则`中，将规则列表规则的情景模式选择为上面全局模式配置的默认情景模式proxy。
	4. 选择`立即更新规则`进行更新规则。

		![gfwlist](https://img.niconode.co/20170226233244355330Nv4HrUK53o5fDm.png)

#### 启动浏览器拓展

![enable](https://img.niconode.co/2017022623351645671j47gvgSiqA5tYvn.png)

- `直接连接` - 不开启任何代理。
- `系统代理` — 如果您希望启用SS客户端上的全局模式，可以直接使用此后再前往启用。
- `proxy` — 使用全局代理，通过客户端的本地端口。
- `auto switch` — 智能切换，只有规则列表中的会智能的自动代理（推荐）。
