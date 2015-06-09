## do-shadowsocks

[![Install on DigitalOcean](http://installer.71m.us/button.svg)][InstallLink]

> 这是一个 [do-install-button](https://github.com/seven1m/do-install-button) 配置，能使用 [DigitalOcean] 快速部署 [Shadowsocks] 服务器。配置脚本基于 [ios-dev-playbook](https://github.com/lexrus/ios-dev-playbook) 实现。虽然用的时候完全不需要知道它们是啥，但是万一遇到问题可以让男朋友传送过去研究一下帮你解决。

[InstallLink]: http://installer.71m.us/install?url=https://github.com/lexrus/do-shadowsocks
[Shadowsocks]: https://github.com/clowwindy/shadowsocks

### 基本要求

1. 一个 [DigitalOcean] 帐号 - 如果你用我的[推广链接](https://www.digitalocean.com/?refcode=3eb5cf371fc9)注册，帐号里马上就能有 10 美刀，如果开 5 美刀的 VPS(512MB 内存)，那就可以免费用两个月了哦
2. [DigitalOcean] 的帐号里有余额或者绑了信用卡可用来建 VPS
3. [DigitalOcean] 里加过 public key - 怎么生成 key 可以看[这里](https://gitcafe.com/GitCafe/Help/wiki/如何安装和设置-Git#2创建-ssh-秘钥)

[DigitalOcean]: https://www.digitalocean.com/?refcode=3eb5cf371fc9

### 安装

点击安装按钮即可开启轻松愉快的安装过程：

[![Install on DigitalOcean](http://installer.71m.us/button.svg)][InstallLink]

如果只装 [Shadowsocks]，用 512MB 完全够用。Region 选 Singapore 和 San Francisco 连接速度都不错。

### 修改默认帐号

记得要记下服务器的 IP 地址，没有记下也可以事后去 [DigitalOcean] 上查看。

安装成功后的默认配置是这样:

- 端口: `5333`
- 加密: `aes-256-cfb`
- 密码: `ilovelex`

如果想改的话，用 ssh 登录这台服务器，修改 `/opt/ss-server/config-default.json` 后，`supervisorctl restart ss-server-default` 重启 [Shadowsocks] 服务。

### 赞助

欢迎请我喝咖啡，我的支付宝帐号是: `lexrus@gmail.com`。

### 相关链接

[do-ikev1](https://github.com/lexrus/do-ikev1) - 在 DigitalOcean 上一键安装 IKEv1 的 VPN。

### 协议

本配置遵循:
```
『有问题问你男朋友』协议
2015 年 修订版
Lex Tang (https://twitter.com/lexrus)

使用者不得任意修改源码中任何一个字符。
使用过程中遇到问题先问谷歌，然后知乎，再问男友。
因正常使用造成的任何损失由男朋友承担。
```
