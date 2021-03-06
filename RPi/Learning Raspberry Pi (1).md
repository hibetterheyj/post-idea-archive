## Learning Raspberry Pi (1)

>Taken Notes from ***Learning Raspberry Pi*** written by **Samarth Shah**

---

### Chapter 1.Getting Started with Raspberry Pi

####  1.1 Different types of operating systems

#####  1.1.1 Different Systems

> [RPi Distributions](https://elinux.org/RPi_Distributions)

- The Raspbian OS

a Linux distribution based on Debian

- The Arch Linux ARM OS

> Official Website: https://wiki.archlinux.org/

1. a port of Arch Linux
2. gives the user a complete control over the system
3. uses the latest software while stability may be a concern

- Pidora

1. Raspberry Pi-optimized remix of Fedora
2. most familiar to OpenSUSE and CentOS users
3. MP3 support and Oracle's Java are not included

- The RISC OS

> Official Website: https://www.riscosopen.org/content/

1. not related to Linux and does not share the Unix lineage
2. a great advantage for time-sensitive tasks and applications where you want to be close to the hardware

- OpenELEC and Raspbmc

1. centered on XBMC
2. a media player that can turn your Raspberry Pi into a **home theater PC** (**HTPC**)

##### 1.1.2 Command summary

**Raspbian**, **Arch** and **Pidora** have similar command lines with few differences.

####  1.2 Installation methods

#####  1.2.1 Preparation

- SD Card

1. using the Class-10 SD card as other Class-4 cards has lots of write failure
2. Class 10 SD Card has faster reading & writing speed than Clas    

#####  1.2.2 Different Methods to Install New System

- NOOBS and BerryBoot
- Installing Raspbian using RAW images

**Expanding the filesystem**

> The detail can check up [this article](https://www.ncnynl.com/archives/201612/1154.html).

####  1.3 User management

> A system running with the default password is not secure 
> as the password is widely known. To avoid this problem, the password needs to 
> be changed.

```
1. First, log in as pi .
2. Then, change the default user password by running the following command:
# passwd
3. Next, enter a root shell by typing this:
# sudo -i
4. Again, run passwd  to change the password. As you are in a root shell, this 
will change the root password this time.
5. Add a new user with a name of your choice by entering the following 
command:
# adduser steve
6. The user will not be able to carry out certain tasks without being a member  
of the relevant groups. The following command will add the user into the 
major groups:
# usermod -a -G  
adm,dialout,cdrom,sudo,audio,video,plugdev,games,users,netdev,  
input,spi,gpio steve
```





