> 该文档最后更新日期: 2018-06-06

<p class="info">我们对本客户端提供「优先」支持</p>

### 介绍

V2RayN 是一个适用于V2Ray-Core的GUI视图化客户端。简单的说，您可以不用自己编辑配置文件与通过命令行运行。

适用协议：`Vmess`

### 下载

版本:2.17 | 更新日期: 2018-10-11

[立即下载](https://dl.niconode.net/client/v2rayN-Core.zip) | [GitHub下载](https://github.com/2dust/v2rayN/releases/download/2.17/v2rayN-Core.zip)

### 运行

- 将您下载的压缩包解压到一个目录。

- 运行其中的 `V2RayN.exe`

	![](https://img.niconode.net/201811070101556923836wVLpgYyFoipZ4.jpg)

### 快速导入

#### 通过链接倒入

- 回到订阅列表，**右键**选择将要添加的线路右侧的 ![](https://img.niconode.net/2018110616132762475fiX1vPnxJp7j6bA.png) 按钮，选择**复制链接地址**。

- 选择 V2RayN 客户端中的左上角`服务器`--`从剪切板倒入批量URL`

> 我们很快会推出批量复制功能，尽情地带

#### 手动添加

- 选择订阅中的`订阅列表`，找到需要添加的线路，选择`获取详细的连接信息`

	![](https://img.niconode.net/2018060611554434584wrF66J5RHF8UoNe.png)

- 显示详细的连接信息，不要关闭窗口。

	![](https://img.niconode.net/2018110701045014967WLQlUq1cR4IZqbZ.jpg)

- 回到 V2RayN 客户端，点击左上角的`服务器`，并选择`添加[Vmess]服务器`，之后将以上所有连接信息逐个复制，并确保一致。

	![](https://img.niconode.net/2018110701060088290PP0XtMYtLmlvACw.jpg)
	
- **请确保底层传输安全中选择了TLS。**

### 选择服务器

- 右键系统右下角托盘中的 V2RayN 客户端的图标。

	![](https://img.niconode.net/2018110701084675813RDxZW7X5qeRDB8x.jpg)
	
### 启动系统代理

- 根据上一步的选择，请可以选择启动HTTP代理，并且在模式中选择以下：

	- 全局模式：所有的网站/程序都将通过代理
	- PAC模式：根据规则匹配
	- 直连模式：仅开启HTTP代理，不设置系统代理。如果您局域网中的其他设备需要连接时（例如PS4、XBox），您可以开启这个选项，并且在其他设备的WIFI设置之高级设置中，设置您电脑的局域网IP，与HTTP代理端口。

如果您只是用于网页浏览，您可以配置到Chrome浏览器中，更智能以及高效率的处理，相见下一节。

### Chrome 浏览器拓展设置

> 您需要现在下载这个拓展，[点击下载](https://dl.niconode.net/extensions/SwitchyOmega.crx) 或 [GitHub下载](https://github.com/FelisCatus/SwitchyOmega/releases/download/v2.3.21/SwitchyOmega.crx)

- 开启开发者模式

- 在您的 Chrome 浏览器中访问 `chrome://extensions/`
	
	![img](https://img.niconode.net/2017022623273770747VNtwGa8iM3BLEj5.png)

- 勾选`开发者模式`

- 安装拓展

- 将刚才下载的`SwitchyOmega.crx`，直接拖动至浏览器窗口。

	![alert](https://img.niconode.net/20170226232840445234N9g1XiHYxUBb4O.png)

- 选择`添加拓展程序`

#### 配置全局模式

- 打开拓展程序首选项，通常来说您的本地端口是`1080`。

- 如下配置默认的情景模式。

	![proxy](https://img.niconode.net/2017022623302525929gbGZc4ylFHjfIJN.png)

- 保存，这个时候您可以使用Chrome中的全局代理功能了。

#### 配置智能模式

- 根据下载进行设置：
	1. 选择`添加规则`。
	2. 在`规则列表列表`中填写`https://raw.githubusercontent.com/gfwlist/gfwlist/master/gfwlist.txt`。
	3. 在`切换规则`中，将规则列表规则的情景模式选择为上面全局模式配置的默认情景模式proxy。
	4. 选择`立即更新规则`进行更新规则。

		![gfwlist](https://img.niconode.net/20170226233244355330Nv4HrUK53o5fDm.png)

#### 启动浏览器拓展

![enable](https://img.niconode.net/2017022623351645671j47gvgSiqA5tYvn.png)

- `直接连接` - 不开启任何代理。
- `系统代理` — 如果您希望启用SS客户端上的全局模式，可以直接使用此后再前往启用。
- `proxy` — 使用全局代理，通过客户端的本地端口。
- `auto switch` — 智能切换，只有规则列表中的会智能的自动代理（推荐）。