> 该文档最后更新日期: 2019-03-27

<p class="info">我们对本客户端提供「优先」支持</p>

### 介绍

V2RayN 是一个适用于V2Ray-Core的GUI视图化客户端。简单的说，您可以不用自己编辑配置文件与通过命令行运行。

适用协议：`Vmess`

### 下载

版本:2.24 | 更新日期: 2019-03-12

[立即下载](https://dl.niconode.co/client/v2rayN-Core.zip) | [GitHub下载](https://github.com/2dust/v2rayN/releases/download/2.24/v2rayN-Core.zip)

### 运行

- 将您下载的压缩包解压到一个目录。

- 运行其中的 `V2RayN.exe`

	![](https://img.niconode.co/201811070101556923836wVLpgYyFoipZ4.jpg)

### 配置订阅

1. 打开您的订阅，选择 `客户端订阅`。找到以 `(API v3.0)` 开始的行列，点击最右边的链接复制。

	![配置文件](https://img.niconode.co/2019032708355416032uJiiVv5gK5MB3BV.png)

2. 打开 V2RayN 客户端，选择 `订阅` 中的 `订阅设置` 。

	![设置订阅地址](https://img.niconode.co/2018120914441597551nmu31FjVvLeAQ9s.png)

3. 在 `地址(url)` 中粘贴 `V2Ray 兼容订阅列表` 的链接地址，并 `确认`。

4. 选择 `订阅` 中的 `更新订阅`。

	![更新订阅](https://img.niconode.co/2018120914450168769ULsZ2NUFfCjE6dK.png "更新订阅")

### 选择服务器

- 右键系统右下角托盘中的 V2RayN 客户端的图标。

	![](https://img.niconode.co/2018110701084675813RDxZW7X5qeRDB8x.jpg)
	
### 启动系统代理

- 根据上一步的选择，请可以选择启动HTTP代理，并且在模式中选择以下：

	- 全局模式：所有的网站/程序都将通过代理
	- PAC模式：根据规则匹配
	- 直连模式：仅开启HTTP代理，不设置系统代理。如果您局域网中的其他设备需要连接时（例如PS4、XBox），您可以开启这个选项，并且在其他设备的WIFI设置之高级设置中，设置您电脑的局域网IP，与HTTP代理端口。

### Chrome 浏览器拓展设置（可选）

<p class="info">以下所有设置为非必要设置，您可根据您的需求进行选择。</p>

如果您只是用于网页浏览，您可以配置到Chrome浏览器中，更智能以及高效率的处理。

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
