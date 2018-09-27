180728一天一技——加快github访问速度

---

https://blog.csdn.net/xinshui151/article/details/79200390

（使用管理员权限）打开记事本后打开`C:\Windows\System32\drivers\etc`处的host文件

```
# GitHub Start 
192.30.253.112 github.com 
192.30.253.119 gist.github.com 
151.101.100.133 assets-cdn.github.com 
151.101.100.133 raw.githubusercontent.com 
151.101.100.133 gist.githubusercontent.com 
151.101.100.133 cloud.githubusercontent.com 
151.101.100.133 camo.githubusercontent.com 
151.101.100.133 avatars0.githubusercontent.com 
151.101.100.133 avatars1.githubusercontent.com 
151.101.100.133 avatars2.githubusercontent.com 
151.101.100.133 avatars3.githubusercontent.com 
151.101.100.133 avatars4.githubusercontent.com 
151.101.100.133 avatars5.githubusercontent.com 
151.101.100.133 avatars6.githubusercontent.com 
151.101.100.133 avatars7.githubusercontent.com 
151.101.100.133 avatars8.githubusercontent.com 
151.101.185.194 github.global.ssl.fastly.net
# GitHub End
```

命令行输入：`ipconfig /flushdns`

---

其他网站加快速度前需查询IP地址：访问https://www.ipaddress.com分别输入github.global.ssl.fastly.net和github.com（范例），得到ip地址

https://blog.csdn.net/xinshui151/article/details/79200390

https://www.cnblogs.com/papi/p/8985581.html