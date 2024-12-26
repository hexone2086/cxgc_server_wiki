file-transform.md
# 文件传输小寄巧

🚫 由于转发隧道采用按流量计费的方式，所以不可以用转发通道进行文件的传输。对于存在的文件传输需求，有目前几个解决方案

## bashupload.com 及其类似网站

try [https://bashupload.com/](https://bashupload.com/)

可以在命令行中上传文件，常用于传输小文件的场景

## 白嫖/付费第三方转发服务

比如说 [sakura frp - https://www.natfrp.com/](https://www.natfrp.com/)

可以根据教程自己建立一个比如说 22 端口的转发服务，然后使用 scp/sftp 传输文件即可.

sakura frp 免费隧道带宽 10M，每天签到可以领 1~4GB 流量，可以凑合用，毕竟是白嫖的...

## 使用 frp 等软件 p2p 打洞

看网络环境随缘，如果 NAT4 基本上可以放弃

以 [frp](https://github.com/fatedier/frp) 举例，自行在服务器端和本机配置运行 frpc，配置参考[点对点内网穿透|frp](https://gofrp.org/zh-cn/docs/examples/xtcp/),其中 server 字段配置请联系管理员索取

如果网络环境正常，默认 STUN 服务器基本可用，不需额外配置

北理在校生推荐使用校园网连接，尽量不要使用移动网络

## BaiduPCS-Py 等云盘工具
- [BaiduPCS-Py](https://github.com/PeterDing/BaiduPCS-Py) 适合氪金大佬，冲SVIP吗🤤

