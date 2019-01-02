---
title: Debian 系统安装 shadowsocks-qt5
date: 2016-12-03
tags: Shadowsocks
categories: 技术
---

终于在 Debian 系统安装使用上了 shadowsocks, 以前尝试安装 command-line-client 失败，这次换 shadowsocks-qt5的.

Github 上[步骤说明](https://github.com/shadowsocks/shadowsocks-qt5/wiki/Installation)比较简单，参考了「[Kali Linux 下安装 Shadowsocks-qt5](http://www.jianshu.com/p/aa48a0a5b30e)」，具体操作记录如下：

1. 安装依赖环境库
```
apt-get install qt5-qmake qtbase5-dev libqrencode-dev libqtshadowsocks-dev libappindicator-dev libzbar-dev libbotan1.10-dev
```
2. git shadowsocks-qt5 源码
 `git clone https://github.com/shadowsocks/shadowsocks-qt5.git`

3.
```
cd shadowsocks-qt5
qmake && make
```

4. `dpkg-buildpackage -uc -us -b`


5. 安装 shadowsocks-qt5

```
dpkg -i ../shadowsocks-qt5-<version>.deb
```


补充说明：

- `libqtshadowsocks-dev` 需要编译安装

 1. `git clone https://github.com/shadowsocks/libQtShadowsocks.git`


 2. `apt-get qtbase5-dev qt5-make qt5-default libbotan1.10-dev unzip debhelper`


 3.
 ```
 cd libQtShadowsocks
 qmake && make   //编译
```


 4. `dpkg-buildpackage -uc -us -b`  //打包

 5. 安装：编译打包好了 3 个安装包在上级目录下
		```
		dpkg -i ../libqtshadowsocks<version>.deb ../libqtshadowsocks-dev<version>.deb
		```


- `apt-get install libzbar-dev` 出错

    > unable locate the package

    解决方法：`aptitude libzbar-dev`

**问题：**

`apt-get install`, `aptitude install`, `dpkg -i` 区别

- `dpkg -i`  主要用来安装已下载好的 .deb 安装包
- `apt-get install` 用来连接网络安装软件，会在软件库中寻找
- `aptitude install` 也用来在线安装软件，但可以解决软件包之间依赖关系

在 APT（advanced packaging tools）中文 wiki 解释里看到有意思的[彩蛋](https://zh.wikipedia.org/wiki/%E9%AB%98%E7%BA%A7%E5%8C%85%E8%A3%85%E5%B7%A5%E5%85%B7#.E5.BD.A9.E8.9B.8B)。

![apt-get moo](https://68.media.tumblr.com/5824bd6a1388c7a42864d25ed96cbae5/tumblr_ohllzs8vdH1uft3xho1_400.png)
![aptitude moo](https://68.media.tumblr.com/241f826fc204c96937d3d0ab3f31cfa1/tumblr_ohllzs8vdH1uft3xho2_400.png)
![apt-build](https://68.media.tumblr.com/cd99f171e35145ea601c414276fb641d/tumblr_ohllzs8vdH1uft3xho3_400.png)
