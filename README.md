# Reality一键安装脚本和各个系统客户端收集推荐

tag:Reality,一键安装脚本,自建翻墙

Trojan特征也很明显，容易被识别，暂时推荐使用Reality自建翻墙代理。下面是一键安装脚本。后面有各个系统的客户端推荐。

本人Telegram电报频道：[科学上网观察与机场测速频道](https://t.me/jichangtj)：掌握最新机场优惠折扣通知，最新机场推荐与机场评测，最新科学上网相关新闻与消息，欢迎关注。

[twitter科学上网与机场观察](https://twitter.com/jichangtj)

<a href="https://jichangpingce.com/ssr-v2ray专线机场推荐.html" target="_blank">20家自用便宜稳定高速国外ssr-v2ray-trojan专线机场推荐</a>


<!--more--> 

## Reality优点

1. 无TLS特征。仍有前向保密性等，且证书链攻击无效，安全性超越常规 TLS
2. 可指向别人的网站，不需要域名。配置 TLS 服务端，更方便，实现向中间人呈现指定 SNI 的全程真实 TLS

禁止回国流量，并转发 TCP/80 和 UDP/443 等端口


[TLS in TLS问题](https://github.com/XTLS/Xray-core/discussions/1295)

[检测 TLS in TLS 的工具](https://github.com/XTLS/Trojan-killer)

不过reality也不是完全安全，墙直接发威 ban整个ip段啥协议都没用。首先得ip干净，比如vultr，甲骨文，谷歌云等这种被重点关注的就很容易被墙。

[Xray REALITY 官方github地址](https://github.com/XTLS/REALITY)


## BBR

买的线路不好的话可以安装BBR加速。

```
wget --no-check-certificate https://github.com/teddysun/across/raw/master/bbr.sh && chmod +x bbr.sh && ./bbr.sh
```
然后重启

## 一键脚本

mack-a大佬的八合一的一键脚本

```
wget -P /root -N --no-check-certificate "https://raw.githubusercontent.com/mack-a/v2ray-agent/master/install.sh" && chmod 700 /root/install.sh && /root/install.sh
```

选择[5.REALITY管理] -- 端口输入443--输入域名最低标准为：国外网站，支持 TLSv1.3 、H2--后面回车即可。

<details>
 <summary>国外网站域名推荐</summary>


gateway.icloud.com
itunes.apple.com
download-installer.cdn.mozilla.net
airbnb【这个不同的区有不同的域名建议自己搜索】
addons.mozilla.org
www.microsoft.com
www.lovelive-anime.jp
www.speedtest.net
www.speedtest.org

# CDN
Apple:
swdist.apple.com
swcdn.apple.com
updates.cdn-apple.com
mensura.cdn-apple.com
osxapps.itunes.apple.com
aod.itunes.apple.com

Microsoft:
cdn-dynmedia-1.microsoft.com
update.microsoft
software.download.prss.microsoft.com

Amazon:
s0.awsstatic.com
d1.awsstatic.com
images-na.ssl-images-amazon.com
m.media-amazon.com
player.live-video.net

Google:
dl.google.com
www.google-analytics.com

</details>


## 客户端推荐

### 安卓/Android

1）[Clash Meta for Android](https://github.com/MetaCubeX/ClashMetaForAndroid) 

A Graphical user interface of Clash.Meta for Android


2）[v2rayNG](https://github.com/2dust/v2rayNG/releases) 

A V2Ray client for Android, support Xray core and v2fly core


3) [NekoBoxForAndroid](https://github.com/MatsuriDayo/NekoBoxForAndroid/releases)

4) clash meta for magisk

[Dashboard 更新发布｜引退](https://t.me/db4cm)

[我是魔改2大王](https://t.me/MagiskChangeKing)

适合想捣鼓的


### Windows

1) [v2rayN](https://github.com/2dust/v2rayN)

Xray-Core需要1.8.1以上

服务器--添加VLESS服务器

<img src="/uploads/reality/xku26x-0.png"  width = "90%"   align=center  alt="v2rayN客户端配置设置教程" />


2）[ClashN](https://github.com/2dust/clashN)

A clash client for Windows, supports Clash core and Clash.Meta core



3）[Clash Verge](https://github.com/zzzgydi/clash-verge/releases)

A Clash GUI based on tauri. Supports Windows, macOS and Linux.



4）[Clash for Windows](https://github.com/Fndroid/clash_for_windows_pkg/releases) 需替换内核为[Clash.Meta](https://github.com/MetaCubeX/Clash.Meta/releases/tag/v1.14.3),内核名字改为clash-darwin。替换文件：clash-win64.exe ，程序目录：resources/static/files/win->x64/



5)[nekoray](https://github.com/MatsuriDayo/nekoray)

### MacOS

1）[Clash Verge](https://github.com/zzzgydi/clash-verge/releases) :A Clash GUI based on tauri. Supports Windows, macOS and Linux.


2）[Clash for Windows](https://github.com/Fndroid/clash_for_windows_pkg/releases) : 同上改内核

替换文件：
intel：/Applications/Clash\ for\ Windows.app/Contents/Resources/static/files/darwin/x64/

ARM（M1、M2）：/Applications/Clash\ for\ Windows.app/Contents/Resources/static/files/darwin/arm64/

3）Wings X

4)[V2RayXS](https://github.com/tzmax/V2RayXS/releases) :GUI for xray-core on macOS



5)[ClashX.Meta](https://github.com/MetaCubeX/ClashX.Meta)



### IOS

1）[Wings X](https://apps.apple.com/app/wings-x/id6446119727)

2）[meta for ios](https://t.me/meta_for_ios)

3）[sing-box](https://sing-box.sagernet.org/installation/clients/sfi/)

4）Shadowrocket：tf版本

### Linux

1）[Clash Verge](https://github.com/zzzgydi/clash-verge/releases)

A Clash GUI based on tauri. Supports Windows, macOS and Linux.


### Openwrt

[ShellClash](https://github.com/juewuy/ShellClash) :通过管理脚本在Shell环境下便捷使用Clash,支持在Shell环境下管理Clash各种功能

[OpenClash](https://github.com/vernesong/OpenClash) :一个可运行在 OpenWrt 上的 Clash 客户端.兼容 Shadowsocks、ShadowsocksR、Vmess、Trojan、Snell 等协议，根据灵活的规则配置实现策略代理

[openwrt-passwall](https://github.com/xiaorouji/openwrt-passwall)

[openwrt-passwall2](https://github.com/xiaorouji/openwrt-passwall2)

[helloworld](https://github.com/fw876/helloworld)

[openwrt-xray](https://github.com/yichya/openwrt-xray) :Prebuilt Xray binaries for OpenWrt



[luci-app-xray](https://github.com/yichya/luci-app-xray) :(Almost) full feature Xray client for OpenWrt


[MerlinClash猫咪爬梯](https://t.me/merlinclashcat) :说明文档：https://mcreadme.gitbook.io/mc


[e58695](https://t.me/e58695/59) : Clash 及其衍生版本均支持 TPROXY 透明代理

[MagiskChangeKing](https://t.me/MagiskChangeKing/126)


### X-UI

xui只是个可视化的配置工具，和一键脚本都差不多，本质还是用的xray

https://github.com/sing-web/x-ui

https://github.com/MHSanaei/3x-ui

https://github.com/FranzKafkaYu/x-ui

**博客来源：**

https://www.v2ray-agent.com/archives/1680104902581

部分来源hostloc网友回复。




