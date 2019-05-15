> 该文档最后更新日期: 2019-05-15

<p class="info">这是一个附加选项，如果您不是为您的游戏加速，您可以不设置该客户端。</p>

### 介绍

SSTap 可以通过创建一个虚拟网卡，之后将所有的流量根据规则转发由 SSTap 处理。

之后 SSTap 会将符合规则的流量转发到代理客户端。

### 下载

版本: 1.1.0.1

[立即下载](https://dl.niconode.co/client/SSTap-beta-setup-1.1.0.1.exe.7z) | [Dropbox 下载](https://www.dropbox.com/s/zx10ytbs5vx19w9/SSTap-beta-setup-1.1.0.1.exe.7z?dl=1)

### 我为什么需要这个？

多数游戏均采用 TCP 或是 UDP 协议进行数据传输。

如果您只是设置了 Clash / V2RayN 客户端，在您玩游戏时，并不会通过我们的线路进行加速。

即便您开了上述客户端的全局模式，这意味着仅处理您所有的HTTP(S)协议的所有数据。

### 我怎么知道改善了？

当您没有设置这个客户端前，即便您连接至了我们的亚洲低延迟线路，您的丢包率与延迟也会偏高。

但在您设置了该客户端后，说明您的流量被全部转发至了 SSTap 处理。

### 为什么设置后延迟还是会在100毫秒左右

因为即便您设置了 SSTap，在您的数据被转发到 SSTap 后，仍需要再转发至代理客户端处理。

这中间会稍微的增加延迟。就像，在冬天时，您穿了多件棉袄，这将会轻微影响您的移动速度。

同样，如果您使用的是无线网络连接，通常也会根据连接信号的强度，而适当的增加20-30毫秒。

> 我们会建议有条件的用户，在路由器上直接设置，但这可能会遇到性能瓶颈。

### 设置步骤

<div class="info">请您确保您在这之前，已经设置完成了 Clash 或 V2RayN 之类的前置客户端。</div>

#### 获取 Clash 客户端的本地代理端口

![](https://img.niconode.co/2019051518071452337lajFaxbajmBqXV2.png)

如图，Port 为 HTTP 代理端口，而 Socks Port 为 Socks5 协议端口。

#### 获取 V2RayN 客户端的本地代理端口

![](https://img.niconode.co/20190515180833771016sTP51izycN8OQZ.png)

打开客户端的 `参数设置`

![](https://img.niconode.co/2019051518085110378ATHpfI9056Ir6PA.png)

如图，本地监听端口为 Socks5 协议端口。

#### 设置 SSTap

![](https://img.niconode.co/20190515180948318695zOfXX9txBQDExe.png)

如图，点击添加按钮。

![](https://img.niconode.co/2019051518103056143J6W7cfdT90NME2U.png)

之后，选择 `添加一个HTTP代理` ，或者 `添加一个Socks5代理`。

> 我们通常建议您添加 Socks5 代理。

![](https://img.niconode.co/2019051518112072394IKU3J94x3QH6lN9.png)

> 参考上图，
>
> 类型 : `SOCKS 5`
>
> 服务器IP : `127.0.0.1`
>
> 端口 : 您客户端的本地代理端口。（参考前面步骤获取）

#### 测试连接

![](https://img.niconode.co/2019051518140431020PTondwqUbhvW3tB.png)

在一切设置完成之后，您可以点击最右侧的小按钮测试连接。

之后，在 `代理` 下拉选中您的游戏，点击下方的 `连接` 按钮。

#### 如果 `代理` 中没有您的游戏？

![](https://img.niconode.co/2019051518154766530rkIdlRBXBNLbncU.png)

在这种情况，我们可以添加一个全局规则，将所有的 TCP+UDP 流量进行处理。

![](https://img.niconode.co/20190515181609898525IlnLehoUV6PeB5.jpg)

参考图片中的值进行填写。

最后，选中您刚刚添加的规则，并连接。

