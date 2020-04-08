# Dell-G3-3579-OpenCore-Boot-File

我的EFI分区备份

Working:

1.支持10.15.4启动。

2.声卡（ALC236）layout-ID=15，工作正常。

3.IGPU（Intel UHD Graphics 630）工作正常。

4.亮度调节正常（Fn+S和Fn+B是快捷键）。

5.默认开启opencore引导菜单，开机-v模式。

6.集成rEFInd和Microsoft Windows10引导项，可正常引导win10，opencore引导项已改为macOS Catalina的标识，有点大，会看不到下面的表示选中的点，属正常现象。

7.WiFi正常（使用DW1820A）。

8.蓝牙正常（使用DW1820A）。

9.OpenCore版本：0.0.4

10.该版本基于Certe Kim所制作的版本，在其之上优化而成。

11.另附GRUB的Shell，使用方法见release中的介绍。

Not Working：

1.DGPU（无解GTX1050Ti），已被SSDT禁用。

2.HDMI（可用适配macOS的USB转HDMI转接线实现外接显示器）。

硬件配置：

CPU:i7-8750H

内存：16GB

无线网卡：DW1820A

IGPU：Intel UHD Graphics 630

DGPU：Nvidia GeForce GTX 1050Ti（Not Working）

注意：

因为整个文件过大，所以我把它放在releases里，1.0版本。
