# Dell G3 3579 OpenCore EFI 引导文件

## 目前由于众所周知的原因，GitHub时常抽风上不了，所以有时更新后可能无法及时发布，gitee会及时更新。gitee地址:https://gitee.com/kp296/dell_g3_3579_opencore_bootloader

## grubx64.efi 用法
setup_var 0x5BC 0x0 (关闭CFG锁)

## 版本更新

### <b><a href="https://github.com/VersionZKP2356/Dell-G3-3579-OpenCore-Boot-File/releases/tag/V6.1">V6.1 OC 0.7.8正式版,通过加入启动参数修复开机黑屏问题</a></b>

<details><summary><b>更早版本</b></summary> 

> <b><a href="https://github.com/VersionZKP2356/Dell-G3-3579-OpenCore-Boot-File/releases/tag/V6.0%2B">V6.0+ OC 0.7.8正式版,实测支持macOS12。修复V6.0中蓝牙问题（2022年2月15日更新)</a></b>

> <b><a href="https://github.com/VersionZKP2356/Dell-G3-3579-OpenCore-Boot-File/releases/tag/V6.0">V6.0 OC 0.7.8正式版,实测支持macOS12。（2022年2月15日更新)</a></b>

> <b><a href="https://github.com/VersionZKP2356/Dell-G3-3579-OpenCore-Boot-File/releases/tag/V5.3">V5.3 OC 0.7.1正式版,不支持macOS12(2021年8月2日更新)</a>

> <b><a href="https://github.com/VersionZKP2356/Dell-G3-3579-OpenCore-Boot-File/releases/tag/V5.2">V5.2 OC 0.7.1正式版,理论支持macOS12(2021年7月30日更新)</a>

> <b><a href="https://github.com/VersionZKP2356/Dell-G3-3579-OpenCore-Boot-File/releases/tag/V5.1">V5.1 OC 0.7.1正式版，修复主题，黑屏问题未完全修复</a></b>(2021年7月7日更新)
  
> <b><a href="https://github.com/VersionZKP2356/Dell-G3-3579-OpenCore-Boot-File/releases/tag/V5.0">V5.0 OC 0.7.1正式版，问题较多，无法显示主题，开机黑屏问题，等待修复。</a></b>(2021年7月6日更新)

> <b><a href="https://github.com/VersionZKP2356/Dell-G3-3579-OpenCore-Boot-File/releases/tag/V4.3">V4.3 OC 0.6.1开发版 修复以太网无法连接网络的问题，无更新kext，注意事项详见release</a></b>(2021年1月31日更新)  

> <b><a href="https://github.com/VersionZKP2356/Dell-G3-3579-OpenCore-Boot-File/releases/tag/V4.2">V4.2 OC 0.6.1开发版 kext更新至12月19日最新版，无大变化</a></b>(2020年12月19日更新)

> <b><a href="https://github.com/VersionZKP2356/Dell-G3-3579-OpenCore-Boot-File/releases/tag/V4.1">V4.1 Preview OC 0.6.1开发版 8月14日编译版(支持Big Sur引导)</a></b>(2020年8月15日更新)

> <b><a href="https://github.com/VersionZKP2356/Dell-G3-3579-OpenCore-Boot-File/releases/tag/V4.0">V4.0 Preview OC 0.6.1开发版(支持Big Sur引导)</a></b>(2020年8月13日更新)

> <b><a href="https://github.com/VersionZKP2356/Dell-G3-3579-OpenCore-Boot-File/releases/tag/V3.0">V3.0 OC 0.6.0正式版(支持Big Sur引导)</a></b>(2020年8月10日更新)

> <b><a href="https://github.com/VersionZKP2356/Dell-G3-3579-OpenCore-Boot-File/releases/tag/V2.0">V2.0 Preview OC 0.6.0开发版(需升级kext才支持big sur)</a></b>(2020年8月10日更新)

> <b><a href="https://github.com/VersionZKP2356/Dell-G3-3579-OpenCore-Boot-File/releases/tag/V1.0">V1.0 OC 0.0.4(带有GRUB Shell)</a></b>(2020年4月8日更新)

</details>

正常工作:

1.支持macOS 12启动。

2.声卡（ALC236）layout-ID=15，工作正常。

3.IGPU（Intel UHD Graphics 630）工作正常。

4.亮度调节正常，原生Fn+F11,Fn+F12.

5.默认开启opencore引导菜单，开机-v模式，<b>2.0版本默认未开启-v跑码，如需开启，请自己添加-v引导参数,其余版本默认开启</b>

6.V2.0及以后版本去除rEFInd,因为我的OpenCore就已经支持引导windows10

7.WiFi正常（使用DW1820A）。

8.蓝牙正常（使用DW1820A）。

9.OpenCore版本：0.7.1正式版

10.在V4.1 Preview之后的版本中，默认加入OC官方GUI引导选择界面，可以用鼠标点选启动项，如不喜欢，具体解除方法见<a href="https://github.com/VersionZKP2356/Dell-G3-3579-OpenCore-Boot-File/releases/tag/V4.1">V4.1 Preview</a>的说明

不工作：

1.DGPU（无解GTX1050Ti），已被SSDT禁用。

2.HDMI（可用适配macOS的USB转HDMI转接线实现外接显示器）。

3.Thunderbolt（未知，因为我电脑没有thunderbolt接口）

硬件配置：

CPU:i7-8750H

内存：16GB

无线网卡：DW1820A

IGPU：Intel UHD Graphics 630

DGPU：Nvidia GeForce GTX 1050Ti(不工作)

  
