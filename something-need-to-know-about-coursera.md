---
title: Coursera应该知道的两三事
tags:
  - 集合汇总
  - Coursera
categories:
  - 技术·小见
toc: true
mathjax: false
comment: true
top: true
date: 2018-06-21 01:03:05
updated: 2018-06-21 01:03:05
thumbnail:
permalink:
top: true
---
<center><font size=5>**Coursera应该知道的两三事**</font></center> 

<center><font size=1>Written by **_PhilHE_** on <u>Jun 21, 2018 </u></font></center> 

<!--more-->

### 说在前面

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;现在越来越多的人使用国外的慕课网站尤其由大名鼎鼎的Andrew Ng创办的**Coursera**来自学各类课程。课程很多，资源很多，而时间有限，想要最大化的去实现较高的学习效率，较好的学习水平，可以通过一些已有的资源、技巧去帮我们make some differences！而一下就是我的一些经验总结，以供参考~

&nbsp;

### 经典课程推荐

`to be continued`

&nbsp;

### 奖学金申请

> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;一直对于Coursera上面很多的课程十分艳羡，但是却没什么动力去一一完成，尤其还没有什么荣誉（关键还是懒），有一次偶然看见姐姐的LinkedIn界面有相关展示，有点怦然心动，便在她的指导下，尝试写下第一篇奖学金申请的表格，与18.06.20正式收到回复，准备在July开课的Robotics: Perception课程进行正式的学习！

#### 奖学金申请问题及其回答：

PS: **首先仅供参考，请注意用英文回答！英文不自信者（如我）可以先谷歌翻译+专有名词翻译+Grammarly拼写检查~**

问题一：**您为何申请助学金？**

I am currently a junior student major Mechatronics Engineer at Tongji Univ. in Shanghai, China. After paying the tuition fee, I do not have much money to cover my living expenses. Moreover, My family is in standard working class so that it is a heavy financial burden on me and my parents. 

In short, that's why I would like to apply for the financial aid. At the same time, I am also looking for an internship in Shanghai. Once I get the job and receive the salary, I think my financial condition would get better.

I would definitely make full use of the financial aid to learn the course well and get myself improved.I will finish the assignments and quiz on time by myself in the course. When I come across some questions and have ideas, I would like to discuss with the peers in the course community and try to contribute my thoughts on the community forums to promote everyone to learn from each other and grow together.

问题一：**学习此课程将如何帮助您实现职业目标？**

First of all, my career goal is to become a robotics scientist. I need to study related courses including mechanics, electronics and computers. Comprehensive mastery and understanding are particularly important for follow-up study and further studies. This course, Robotics: Perception, is well-rated and highly professional so I believe it will help finally.

Second, I want to accept online courses in the future because this is a good way to learn knowledge and English at the same time. I will continue to study at Cousera. When I take the course, I will finish my homework and quiz on time. I will discuss with the peers in the course community when encountering some problems. If necessary, I will also publish my ideas on the community forum.

Last but not least, the course certificate is a short-term goal for myself so that it can inspire me to study this course. On the other hand, the course certificate will also increase the value of my Linkedin Profile and resume. It can prove that I am a life-long learner.

#### 奖学金申请其他问题

`to be continued`

&nbsp;

### 下载神器：coursera-dl

> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;我们在墙内总会遇上问题，而这其中最主要的就是**网站、视频访问速度太慢**，随之而来的解决方法就是利用小技巧<u>将讲义、视频还有字幕文件下载下来</u>。此方法还能方便本地随时查看，减小因网络限制带来的影响！

#### 安装与更新

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;经过多次跳坑试坑，最终确定[知乎：如何批量下载 Coursera 视频、字幕、教材？-- Li Ming 的回答](https://www.zhihu.com/question/24630418/answer/142576655) 方为正确的操作，而目前较为高票的回，偏听则暗啊！）

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;前置条件为*Python*的安装，建议为较新的Python3.X版本。成功安装Python后，以管理员权限打开命令行**cmd**输入`pip install coursera-dl`，慢慢等待下载的完成。

#### 使用与进阶

- **1.（是否管理员权限皆可）打开命令行cmd输入以下代码,下载地址为命令行打开地址，命令行内容可以简单查看[我的命令行入门笔记](http://localhost:4000/2017/08/20/after-reading-the-command-line-crash-course/)。**

`coursera-dl -u 用户名 -p 登陆密码 课程名称`

- **2.什么是课程名称？&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;点开想学习的课程(我一般注册课程后下载)，查看它的网址，比如最出名的Andrew Ng的机器学习课程网址**

```
http://www.coursera.org/learn/machine-learning 
%本课程名称即为learn以后的一段内容：machine-learning 
```

- **3.所以输入命令行即为**

`coursera-dl -u your_username -p your_password machine-learning`

- **4.最后也是最重要的一步——由于种种原因，下载未能完全（比如我就遇到只下载了讲义，无法成功下载视频的情形），那么则需要更新电脑的host文件，避免GFW的DNS污染（天朝真是威武！），网址详见[相关网址](https://jingyan.baidu.com/article/6f2f55a14059eeb5b93e6cab.html)。**

- **5.进阶操作**

```
coursera-dl -u <user> -p <pass> 课程名称
% 一般操作          

coursera-dl -u <user> -p <pass> 课程1 课程2 ... 课程n
% Multiple classes多课程一起下

coursera-dl -u <user> -p <pass> -f "ppt" qcomp-2012-001
% Download only ppt files: 只下某一类型如ppt    

coursera-dl -n -b ni-001
% Get the preview classes:下载课程预览?     

coursera-dl -n --path=C:\Coursera\Classes\ comnetworks-002
% Specify download path: 下载位置      

coursera-dl --help
%Display help:  显示帮助              
```

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;更多选项请参考项目[github页面](https://github.com/coursera-dl/coursera-dl)。




&nbsp;
&nbsp;
（最后更新于*2018.06.21*）