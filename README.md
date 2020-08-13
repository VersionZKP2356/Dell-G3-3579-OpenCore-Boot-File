# Dell-G3-3579-OpenCore-Boot-File

# <b>当前最新正式版本是<a href="https://github.com/VersionZKP2356/Dell-G3-3579-OpenCore-Boot-File/releases/tag/V2.0">V2.0</a>！！！<b>

正常工作:

1.支持<s>10.15.4</s> 11 Big Sur和10.13.6启动。

2.声卡（ALC236）layout-ID=15，工作正常。

3.IGPU（Intel UHD Graphics 630）工作正常。

4.亮度调节正常（Fn+S和Fn+B是快捷键）。

5.默认开启opencore引导菜单，开机-v模式，<b>2.0版本默认未开启-v跑码，如需开启，请自己添加-v引导参数</b>

6.<s>集成rEFInd和Microsoft Windows10引导项，可正常引导win10，opencore引导项已改为macOS Catalina的标识，有点大，会看不到下面的表示选中的点，属正常现象。</s>  2.0及以后版本去除rEFInd,因为我的OpenCore就已经支持引导windows10

7.WiFi正常（使用DW1820A）。

8.蓝牙正常（使用DW1820A）。

9.OpenCore版本：<s>0.0.4</s>  最新0.6.0正式版，还有0.6.1开发版

10.另附GRUB的Shell(仅在<a href="https://github.com/VersionZKP2356/Dell-G3-3579-OpenCore-Boot-File/releases/tag/v1.0">1.0</a>版本中有)，使用方法见release中的介绍。

不工作：

1.DGPU（无解GTX1050Ti），已被SSDT禁用。

2.HDMI（可用适配macOS的USB转HDMI转接线实现外接显示器）。

3.Thubderbolt（未知，因为我电脑没有thunderbolt接口）

硬件配置：

CPU:i7-8750H

内存：16GB

无线网卡：DW1820A

IGPU：Intel UHD Graphics 630

DGPU：Nvidia GeForce GTX 1050Ti（Not Working）

注意：

因为整个文件过大，所以我把它放在releases里，<s>1.0版本</s>  最新版本2.0，3.0版是OC0.6.0开发版，比0.6.0正式版版本要低，<s>如果我有时间我会再出一个0.6.1开发版，敬请期待</s>

0.6.1开发版已经放出，在<a href="https://github.com/VersionZKP2356/Dell-G3-3579-OpenCore-Boot-File/releases/tag/V4.0">V4.0 Preview</a>

