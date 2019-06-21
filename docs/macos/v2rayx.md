> 该文档最后更新日期: 2019-06-20

<p class="info">我们对本客户端提供「优先」支持</p>

## 介绍

V2Ray X是一款社区开源型GUI客户端，用于控制V2Ray-Core 以连接V2Ray 服务。

适用协议：`V2Ray`

## 下载

版本号：1.5.1 | 更新日期: 2019-02-13

[立即下载](https://dl.niconode.co/client/V2RayX.app.zip) | [Github下载](https://github.com/Cenmrev/V2RayX/releases/download/v1.5.1/V2RayX.app.zip)

## 手动添加

- 打开`订阅列表`，选择线路右边的`获取详细连接信息`。

	![](https://img.niconode.co/2018060611554434584wrF66J5RHF8UoNe.png)

- 选择托盘中的 V2RayX，选择`Server`

	![](https://img.niconode.co/2018060614090518999jkUFg39A9Ousnyg.png)

- 根据连接信息中，一个一个复制粘贴，确保信息一致。

	![](https://img.niconode.co/2018060614095842623BQEtYFVODoM0Dxc.png)

### 开启 TLS

- 选择 `transport settings`

	![](https://img.niconode.co/2018110504030133949IcV8mqmvZOefCjA.png)
	
- 打开 TLS 选项卡，勾选 `Use TLS`，并在 `Server Name` 中天蝎我们的服务地址。

	**请确保服务器地址完全一致，否则将无法连接我们的服务**

	![](https://img.niconode.co/20181105040345809354VH9VdAZbvOFIm3.png)

## 开始连接

- 选择托盘中的 V2RayX，选择`Server`

	![](https://img.niconode.co/2018060614090518999jkUFg39A9Ousnyg.png)

	- 确保V2Ray: On，如果不是，则点击Start V2Ray
	- V2Ray Rule - 根据V2Ray规则代理
	- PAC Rule - 根据PAC规则代理(推荐)
	- Global Mode - 全局模式
	- Manual Mode - 手动模式（不启用系统代理）

## 配合 Surge 使用

- 选择 Manual Mode，默认情况下，V2Ray X本地监听信息如下：

	|类型|端口|
	|---|---|
	|Socks5|1081|
	|HTTP|8001|
	
- 打开 Proxies 代理 选项卡

- 添加一个新的代理，信息如下：

	![](https://img.niconode.co/2018110504113875927KuDEQYj4Hu3e68A.png)

- 保存后，点击Surge，下拉的服务器选择刚刚创建的V2Ray

	![](https://img.niconode.co/2018110504135320926v5gczuAYKKaBWTy.png)
	
- 在Outbound Mode选择最后一个，即可继续使用您原先的Surge规则了。

- **如果您要切换服务器，清前往V2RayX 客户端中的服务器列表进行选择**
