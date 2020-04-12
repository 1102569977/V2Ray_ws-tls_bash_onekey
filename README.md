## V4Ray 基于 Nginx 的 vmess+ws+tls 一键安装脚本

> 感谢 JetBrains 提供的非商业开源软件开发授权

> Thanks for non-commercial open source development authorization by JetBrains
### 个人备份专用，使用本脚本，后果自负！
* 个人备份专用，使用本脚本，后果自负！
* 个人备份专用，使用本脚本，后果自负！

### 最高机密
* 准备一个域名，并将YOUXIANG记录添加好。
* 不知道，这下面是什么！
* 安装 wget ：apt install wget -y

### 安装/更新方式（h2 和 ws 版本已合并）
Vmess+websocket+TLS+Nginx+Website
```
wget -N --no-check-certificate -q -O install.sh "https://raw.githubusercontent.com/1102569977/V2Ray_ws-tls_bash_onekey/master/install.sh" && chmod +x install.sh && bash install.sh
```

### 注意事项
* 个人备份专用，使用本脚本，后果自负！
*个人备份专用，使用本脚本，后果自负！
*个人备份专用，使用本脚本，后果自负！
### 更新日志
> 没有自动拉取！

### 鸣谢
* 感谢脚本中的作者！备份不记名！
* 感谢脚本中的作者！备份不记名！
* 感谢脚本中的作者！备份不记名！
* 感谢脚本中的作者！备份不记名！

### 证书
> 需要博士毕业证书才能看懂！

脚本支持自动生成毕业证书！

### 查看客户端配置
`cat ~/v2ray_info.txt`

### V4ray 简介

* V4Ray是一个优秀的开源网络代理工具，可以帮助你畅爽体验互联网，目前已经全平台支持Windows、Mac、Android、IOS、Linux等操作系统的使用。
* 本脚本为一键完全配置脚本，在所有流程正常运行完毕后，直接按照输出结果设置客户端即可使用
* 请注意：我们依然强烈建议你全方面的了解整个程序的工作流程及原理

### 建议单服务器仅搭建单个代理
* 本脚本默认安装最新版本的V4ray core
* V4ray core 目前最新版本为 4.22.1（同时请注意客户端 core 的同步更新，需要保证客户端内核版本 >= 服务端内核版本）
* 建议使用默认的443端口作为连接端口
* 伪装内容可自行替换。

### 注意事项
* 推荐在纯净环境下使用本脚本，如果你是新手，请不要使用Centos系统。
* 在尝试本脚本确实可用之前，请不要将本程序应用于生产环境中。
* 该程序依赖 Nginx 实现相关功能，请使用 [LNMP](https://lnmp.org) 或其他类似携带 Nginx 脚本安装过 Nginx 的用户特别留意，使用本脚本可能会导致无法预知的错误（未测试，若存在，后续版本可能会处理本问题）。
* V4Ray 的部分功能依赖于系统时间，请确保您使用V2RAY程序的系统 UTC 时间误差在三分钟之内，时区无关。
* 本 bash 依赖于 [V4ray 官方安装脚本](https://install.direct/go.sh) 及 [acme.sh](https://github.com/Neilpang/acme.sh) 工作。
* Centos 系统用户请预先在防火墙中放行程序相关端口（默认：80，443）


### 启动方式

启动 V4ray：`systemctl start v2ray`

停止 V4ray：`systemctl stop v2ray`

启动 Nginx：`systemctl start nginx`

停止 Nginx：`systemctl stop nginx`

### 相关目录

Web 目录：`/home/wwwroot/3DCEList`

V4ray 服务端配置：`/etc/v2ray/config.json`

V4ray 客户端配置: `~/v2ray_info.inf`

Nginx 目录： `/etc/nginx`

证书文件: `/data/v2ray.key 和 /data/v2ray.crt` 请注意证书权限设置

### 捐赠

脚本作者的aff：https://iceyun.top/auth/register?code=qwsV


