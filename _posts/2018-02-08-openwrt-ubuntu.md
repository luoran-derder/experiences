---
layout: default
title: Ubuntu(sever)下搭建openwrt
---

<h2>{{ page.title }}</h2>
<p>
       首先要对整个系统有一定的了解，大体知道基本框架。ubuntu是以linux系统的一个开源发行版，ubuntu相比于linux就像win7相比于windows(我相信这样的比喻大家比较好理解)，让ubuntu运行起来需要安装虚拟机(vmware或virtual box)，虚拟机部署完成后，恭喜你，你将会有两个操作系统(一个是windows，另外一个是虚拟机上的ubuntu)，接下来我们要在openwrt官网上下载源码到ubuntu，接着编译，编译完成后，会生成我们需要的固件。将固件烧录到openwrt板子上(其实这个固件类似于openwrt板子的操作系统)，最后一步就是配置路由器了(一种是通过ssh登录用命令行控制，一种是登陆web界面用web控制)，至此，openwrtn板子已经能够运行了，但是就像手机一样，没了应用程序什么都办不了，所以我们还要开发openwrt的应用软件(一种是利用OpenWrt SDK,一种是利用OpenWrt源码)。这就是开发openbwrt的整个流程，我只写整体的思路和框架，当然在实际中还会遇到很多很多麻烦，需要大家谷歌百度自行解决。接下来我会分步骤详细介绍。</p>
## title one ：搭建开发环境
 
<p>sudo apt-get install g++ </p>
<p>sudo apt-get install libncurses5-dev</p>
sudo apt-get install zlib1g-dev
sudo apt-get install bison
sudo apt-get install flex
sudo apt-get install unzip
sudo apt-get install autoconf
sudo apt-get install gawk
sudo apt-get install make
sudo apt-get install gettext
sudo apt-get install gcc
sudo apt-get install binutils
sudo apt-get install patch
sudo apt-get install bzip2
sudo apt-get install libz-dev
sudo apt-get install asciidoc
sudo apt-get install subversion
sudo apt-get install sphinxsearch
sudo apt-get install libtool
sudo apt-get install sphinx-common







<p>{{ page.date | date_to_string }}</p>
