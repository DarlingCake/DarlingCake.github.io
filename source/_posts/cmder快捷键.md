---
title: cmder快捷键
date: 2019-02-06 21:46:54
tags: 常用软件快捷键
---

1. Cmder常用快捷键

2. - Tab：自动路径补全
   - ctrl+T:建立新页签
   - ctrl+W：关闭页签
   - ctrl+tab：切换页签
   - alt_f4:关闭所有页签
   - alt+shift+1:开启cmd.exe
   - alt+shift+2:开启powershell.exe
   - alt+shift+3:开启powershell.exe（系统管理员权限）
   - ctrl+1:快速切换到第一个页签
   - ctrl+n:快速切换到第n个页签
   - alt+enter:切换到全屏状态
   - ctrl+r:历史命令搜索

3. 可在视窗内搜寻画面上曾经出现过的任意字

4. 新增页签按钮，可透过滑鼠新增页签

5. 切换页签按钮，可透过滑鼠切换页签

6. 锁定视窗，让视窗无法再输入

7. 切换视窗是否提供卷轴功能，启动时可查询之前显示过的内容

8. 按下滑鼠左键可开启系统菜单，滑鼠右键可开启工具选项视窗，win+alt+p开启工具选项视窗。



### Chocolatey软件包管理系统

在 Linux 下，大家喜欢用apt-get(mac下用brew)来安装应用程序，如今在 windows 下，大家可以使用Chocolatey来快速下载搭建一个开发环境。Chocolatey的哲学就是完全用命令行来安装应用程序， 它更像一个包管理工具（背后使用Nuget）

另外需要说明的是，Chocolatey只是把官方下载路径封装到了Chocolatey中，所以下载源都是其官方路径，所以下载的一定是合法的，但是如果原软件是需要 Licence 注册的话，那么Chocolatey下载安装好的软件还是需要你去购买注册。不过Chocolatey一般还是会选用免费 Licence 可用的软件。

安装chocolatey , 运行如下命令即可：

@powershell -NoProfile -ExecutionPolicy unrestricted -Command "iex ((new-object net.webclient).DownloadString('<https://chocolatey.org/install.ps1>'))" && SET PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin



安装软件命令choco install softwareName, 短写是cinst softwareName可安装的应用程序，可以参见其 Package列表



以下是window下开发常用的开发环境应用:



- choco install autohotkey.portable #安装 AutoHotkey (Portable) 

- choco install nodejs.install #安装 node 

- choco install git.install #安装 git 

- choco install ruby #安装 ruby 

- choco install python #安装 python 

- choco install jdk8 #安装 JDK8 

- choco install googlechrome #安装 Chrome 

- choco install google-chrome-x64 #Google Chrome (64-bit only) 

- choco install firefox #安装 firefox 

- choco install notepadplusplus.install #安装 notepad++ 

- choco install Atom #安装 Atom 

- choco install SublimeText3 #安装 SublimeText3