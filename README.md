# Actions-OpenWrt

[![LICENSE](https://img.shields.io/github/license/mashape/apistatus.svg?style=flat-square&label=LICENSE)](https://github.com/P3TERX/Actions-OpenWrt/blob/master/LICENSE)
![GitHub Stars](https://img.shields.io/github/stars/P3TERX/Actions-OpenWrt.svg?style=flat-square&label=Stars&logo=github)
![GitHub Forks](https://img.shields.io/github/forks/P3TERX/Actions-OpenWrt.svg?style=flat-square&label=Forks&logo=github)

Build OpenWrt using GitHub Actions

[Read the details in my blog (in Chinese) | 中文教程](https://p3terx.com/archives/build-openwrt-with-github-actions.html)

NEWIFI3
自动从lean的lede源码clone并生成newifi3固件

由于源码更新升级内核和更换了大量软件包，但此仓库配置文件为旧文件，若出现问题请在issue反馈

目前使用的是开源驱动，若需要使用闭源驱动，请按以下说明更改配置

CONFIG_PACKAGE_kmod-mt7603=y        #取消选中该包
CONFIG_PACKAGE_kmod-mt7603e=n       #选中该包
CONFIG_PACKAGE_kmod-mt76x2=y        #取消选中该包
CONFIG_PACKAGE_kmod-mt76x2-common=y #取消选中该包
CONFIG_PACKAGE_kmod-mt76x2e=n       #选中该包

CONFIG_PACKAGE_luci-app-mtwifi=n    #选中该包
=============================================

本仓库每天UTC 20:00自动拉取源码编译，可直接在action中下载最新固件

Build Newifi 3

固件具体更新内容移步到 https://github.com/coolsnowwolf/lede 查看

固件的默认地址为192.168.99.1，密码默认password
