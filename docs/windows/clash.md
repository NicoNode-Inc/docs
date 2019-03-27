> 该文档最后更新日期: 2019-03-27

<p class="info">我们对本客户端提供「优先」支持</p>

### 介绍

Clash 是一个适用于V2Ray的GUI视图化客户端。简单的说，您可以不用自己编辑配置文件，同时还可以进行丰富的规则订阅与设置。

适用协议：`Vmess`

### 下载

版本: 0.5.30 | 更新日期: 2019-03-19

[立即下载](https://dl.niconode.co/client/Clash.for.Windows.Setup.0.5.30.exe) | [GitHub下载](https://github.com/Fndroid/clash_for_windows_pkg/releases/download/0.5.30/Clash.for.Windows.Setup.0.5.30.exe)

### 配置订阅

1. 打开您的订阅，选择 `客户端订阅`。找到以 `(API v3.2)` 开始的行列，点击最右边的链接复制。

	![配置订阅](https://img.niconode.co/2019032708301910942SJ1XCgEkvGQfa7k.png)
	
2. 打开 Clash 客户端，选择 `Profiles`，在底部左侧的`Download remote configuration file (下载远程配置文件)` 中，粘贴  `Clash Mac/Win` 的链接地址，选择 `Download (下载)`。

3. 下载完成后，前往 `General （基本)`，将底部的 `System Proxy (系统代理)` 勾选启用。

	![启用系统代理](https://img.niconode.co/2018120914564660326t4l6LI22NGL0lEw.jpg)

### 切换模式/线路

- 前往 `Proxies (代理)` 标签卡。

	![切换模式/线路](https://img.niconode.co/20181209145907166196gyJqiCYh6aW3iz.jpg)
	
- 在最顶部的三个按钮中，分别为：
	- Global 全局模式：所有的连接/网站都将通过我们的服务
	- Rule 规则模式：将根据我们为您提供的规则，智能识别站站点，能够正常访问的站点将不通过我们的服务。
	- Direct 直连模式：不连接至我们的服务。

- 切换服务器：
	- 您可以直接在 `Proxy` 或 `GLOBAL` 中选择服务器。
	- 当您启用 `Rule` 模式时，您可以单独选择 `Netflix` 分组里的线路以切换不同的 Netflix 分区。
	
> 小提示：您可以先选择右上角的 `Test Letency` 进行延迟测试，之后选择数值最低的线路。
