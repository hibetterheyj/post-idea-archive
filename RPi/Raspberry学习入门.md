[TOC]

# Raspberry学习

> 官方文档：
>
> [Raspberry Pi Hardware Guide](https://www.raspberrypi.org/learning/hardware-guide/)
>
> [Raspberry Pi Software Guide](https://www.raspberrypi.org/learning/software-guide/)
>
> 其他：
>
> [RPi Tutorials](https://elinux.org/RPi_Tutorials)

##  教程

###  （教程、树莓派）

####  [I.入门介绍](https://www.bilibili.com/video/av18821107)

必买配件：

- 主板，最新
- SD卡，最小8G
- 读卡器
- 网线
- 散热片
- 保护外壳
- 开关电源线

选买：

- 传感器
- GPIO引脚拓展坞

软件：

SourceForge

- SD formattor
- Win32 Disk Imager 用于写入官方镜像
- putty 连接方式
- 连接wifi Console-ifconfig-IP地址
- pi@raspberry
- sudo raspi-config 进行相关配置
- IOT: [node-red](https://segmentfault.com/a/1190000008603115)

####  [II.系统安装，ssh](https://www.bilibili.com/video/av18821107)

- 安装可视化桌面

1. 格式化SD卡 **SD Formatter**
2. 烧录系统 **Win32 Disk Imager**
3. 配置ssh，配置wifi **VS Code**
4. 远程登陆配置 **putty**
5. 寻找IP **ipscan**
6. 远程桌面实现 **realvnc-vnc-server, realvnc-vnc-viewer**
7. 手机/电脑查看 **VNC Viewer**

待完成：

1. 配置国内软件源，可以不需要下载tightvncserver

- 配置wifi

```bash
ifconfig
sudo nano /etc/wpa_supplicant/wpa_supplicant.conf
% 添加下述内容
network={
ssid="A204"
psk="dachuangjidi"
key_mgmt=WPA-PSK
priority=1
scan_ssid=1
}

Crtl+X                  exit the file
Y                       yes, and save it
enter                   get out to terminal
sudo shutdown -h now    shutdown the RPi
```

- 固定IP

```
% 登陆后启动输入
vncserver :1
% 从动态变为静态IP的过程（待补充）
```

