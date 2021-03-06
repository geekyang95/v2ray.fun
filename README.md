术业有专攻，一部分人一辈子都不会搞懂这些网络，但是他们仍然有权利自由地访问互联网，懂技术的人不一定可以通过技术改变世界。

<!-- vim-markdown-toc GFM -->

* [V2ray.fun](#v2rayfun)
    * [功能](#功能)
    * [安装命令](#安装命令)
    * [升级命令](#升级命令)
    * [卸载命令](#卸载命令)
    * [截图](#截图)
    * [系统要求](#系统要求)
    * [软件要求](#软件要求)
    * [更新日志](#更新日志)
    * [特别说明](#特别说明)
* [Buy me a coffee](#buy-me-a-coffee)

<!-- vim-markdown-toc -->

# V2ray.fun

V2ray控制脚本，向导式更改端口，加密方式，传输协议，享受V2ray的乐趣~


## 功能

- 一键 启动 / 停止 / 重启 V2ray 服务端
- 自动随机生成 UUID
- 自助修改端口
- 快速查看服务器连接信息
- 一键下载客户端配置文件和**二维码**（通过szrz程序，xshell，secureCRT还有[macOS的iterm2](https://github.com/tracyone/v2ray.fun/wiki/MAC使用RZ、SZ远程上传下载文件都支持)都支持）
- 自由更改**传输配置**：
  - 常规TCP
  - HTTP头部伪装
  - WebSocket流量
  - 常规mKCP流量
  - mKCP 伪装 FaceTime通话流量
  - mKCP 伪装 BT下载流量
  - mKCP 伪装 微信视频通话流量

**WebSocket不包括Nginx分流，请自行安装Nginx来分流。**

## 安装命令

```bash
bash -c "$(curl -fsSL https://git.io/fh9As)"
```

## 升级命令
```bash
bash -c "$(curl -fsSL https://git.io/fh9AZ)"
```

## 卸载命令
```bash
bash -c "$(curl -fsSL https://git.io/fh9AC)"
```


## 截图

![1](1.png)

![2](2.png)

![3](3.png)

![4](4.png)

## 系统要求

- Debian 7 
- **Debian 8（推荐）**
- Ubuntu 14 
- Ubuntu 16 
- CentOS 7

**不支持Centos 6**

## 软件要求

请使用**Xshell**连接服务器，以获得完美的中文支持以及配置文件下载功能。

## 更新日志

**2017.9.4**
第一版通过测试发布。

**2017.10.16**
新增TLS功能，自动获取证书。

**2018.5.1**

- 支持修改alterID
- 支持动态端口的使能和禁止

**2018.6.11**
- 支持修改动态端口的范围
- 增加菜单：更新v2ray以及v2ray.fun

**2018.7.7**

- 支持生成v2rayN(windows以及安卓) & Pepi(IOS) 客户端的
vmess链接和qrcode图片，支持通过用sz将qr图片传到本机。

**2019.2.7**

- 由tracyone接手的v2ray.fun项目已被删除，本人稍作修改暂可继续使用。
<b>Attention!</b>
如果您安装了之前由tracyone编写的项目，请不要贸然使用全新安装的方式升级，否则会使您当前安装的v2ray配置文件被重设以至于无法正常工作！

**2019.2.17**

- 修改广告过滤功能实现的方式，将v2ray所依赖的 config.json 配置文件中冗长的域名列表去除，采用外挂[ToutyRater](https://github.com/ToutyRater) 制作的 h2y.dat 文件中的广告过滤规则，不但减轻了操作 config.json 文件的压力，还让广告过滤列表可以随时方便地更新。[项目地址](https://github.com/ToutyRater/V2Ray-SiteDAT)
- 经测试，动态多端口功能并不能有效提高对 GFW 的欺骗，故将该功能设置为默认关闭的状态。

## 特别说明

也可以先查看下本仓库的[wiki](https://github.com/leitbogioro/v2ray.fun/wiki)

本程序遵循 GPL v3协议发布，请Fork保留源项目地址，谢谢！

V2ray : [https://v2ray.com](https://v2ray.com)

一代目（已转型，正开发全新的v2ray.fun项目: https://github.com/FunctionClub/V2ray.Fun）: [雨落无声](https://github.com/YLWS-4617)

二代目（已引退）: [tracyone](https://github.com/tracyone)

三代目（在服役）: [leitbogioro](https://github.com/leitbogioro)
