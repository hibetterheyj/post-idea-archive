## 一天一技 - chrome上配置SwitchyOmega

---

> [Shadowsocks服务器配置可用,chrome(google浏览器)无法连接上网，用SwitchyOmega插件设置代理](https://blog.csdn.net/qq_38410428/article/details/82260552#commentsedit)

- 下载SwitchyOmega插件（下载地址<https://pan.baidu.com/s/19y8rEqeKY7E7orjLxulqAA>），OmegaOptions插件（下载地址<https://pan.baidu.com/s/1YU6WM7P10Mg8h7dLHUxqSg>）。SwitchyOmega插件也可以从chrome商店中直接下载，OmegaOptions插件可以自动检测PAC模式和全局模式即auto switch模式。
- 然后点击google浏览器右上角的图标，找到‘更多工具’中的‘扩展程序’，然后将Proxy-SwitchyOmega-Chromium-2.5.15.crx 移动到扩展程序上面去。（如果显示无法移动脚本，可以在chrome商店中下载Proxy-SwitchyOmega，chrome会自动安装） 

![1](C:\Users\admin\Desktop\翻墙related\1.png)

![2](C:\Users\admin\Desktop\翻墙related\2.png)

![3](C:\Users\admin\Desktop\翻墙related\3.png)

- 点击proxy,将代理协议改为SOCKS5，代理服务器改为127.0.0.1（本机地址），代理端口为1080，然后点击应用选项，此时全局代理模式已经启动，重启ss系统代理，选择全局代理模式即可上Google浏览器。 

![4](C:\Users\admin\Desktop\翻墙related\4.png)

- 由于上述为全局模式即只要打开网页都是用VPN翻墙，上网速度比较慢，所以用OmegaOptions.bak进入PAC模式（可以自动检测是否需要翻墙，提高上网速度）
- 点击‘导入/导出’，选择‘从备份文件恢复’，选择文件OmegaOptions.bak，然后‘应用选项’即可。 

![5](C:\Users\admin\Desktop\翻墙related\5.png)

- 点击Google浏览器右上方的绿色圆圈，就可以对proxy（全局模式）和auto switch（PAC模式）两种模式进行切换。 

![6](C:\Users\admin\Desktop\翻墙related\6.png)

![7](C:\Users\admin\Desktop\翻墙related\7.png)

# 全局模式和PAC模式有什么不同

1. 全局模式速度比PAC模式速度慢很多，一般都是开PAC模式。
2. 全局模式每个浏览器的ip地址都是本机代理服务器的ip地址。 
3. PAC模式中Google浏览器是代理服务器的地址，不用翻墙的浏览器是所用公共网的地址。 

