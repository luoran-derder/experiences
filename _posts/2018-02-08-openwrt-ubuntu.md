---
layout: default
title: Ubuntu(sever)下搭建openwrt
---

<h2>{{ page.title }}</h2>
<p>
       首先要对整个系统有一定的了解，大体知道基本框架。ubuntu是以linux系统的一个开源发行版，ubuntu相比于linux就像win7相比于windows(我相信这样的比喻大家比较好理解)，让ubuntu运行起来需要安装虚拟机(vmware或virtual box)，虚拟机部署完成后，恭喜你，你将会有两个操作系统(一个是windows，另外一个是虚拟机上的ubuntu)，接下来我们要在openwrt官网上下载源码到ubuntu，接着编译，编译完成后，会生成我们需要的固件。将固件烧录到openwrt板子上(其实这个固件类似于openwrt板子的操作系统)，最后一步就是配置路由器了(一种是通过ssh登录用命令行控制，一种是登陆web界面用web控制)，至此，openwrtn板子已经能够运行了，但是就像手机一样，没了应用程序什么都办不了，所以我们还要开发openwrt的应用软件(一种是利用OpenWrt SDK,一种是利用OpenWrt源码)。这就是开发openbwrt的整个流程，我只写整体的思路和框架，当然在实际中还会遇到很多很多麻烦，需要大家谷歌百度自行解决。接下来我会分步骤详细介绍。</p>
## title one ：搭建开发环境
 虚拟机安装好以后(物理机也行),还需要下载所依赖的库文件才能正常编译(以下命令需要小伙伴了解linux命令行)
<p>sudo apt-get install g++ </p>
<p>sudo apt-get install libncurses5-dev</p>
<p>sudo apt-get install zlib1g-dev</p>
<p>sudo apt-get install bison</p>
<p>sudo apt-get install flex</p>
<p>sudo apt-get install unzip</p>
<p>sudo apt-get install autoconf</p>
<p>sudo apt-get install gawk</p>
<p>sudo apt-get install make</p>
<p>sudo apt-get install gettext</p>
<p>sudo apt-get install gcc</p>
<p>sudo apt-get install binutils</p>
<p>sudo apt-get install patch</p>
<p>sudo apt-get install bzip2</p>
<p>sudo apt-get install libz-dev</p>
<p>sudo apt-get install asciidoc</p>
<p>sudo apt-get install subversion</p>
<p>sudo apt-get install sphinxsearch</p>
<p>sudo apt-get install libtool</p>
<p>sudo apt-get install sphinx-common</p>
<p>sudo apt-get install git-core</p>
## title two : 在openwrt官网下载源码(https://openwrt.org/)
<p>在ubuntu上调用命令直接安装，如果不熟悉命令的小伙伴，请自行学习</p>
## title three : 编译openwrt源码
<p>配置编译环境:$ make menuconfig</p> 
<p>输入以上命令之后，会进入一个命令行图形界面</p>

[*]表示:这个包裹选中编译，并安装在升级版本中； 
[M]表示：这个软件包选中编译，但并不安装在升级版本中
 
 <p>{{ page.date | date_to_string }}</p>
