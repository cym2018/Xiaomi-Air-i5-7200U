# 小米笔记本Air 13.3 7代黑苹果配置

支持的版本：

* macOS Mojave 10.14.5 (18F132)

* macOS Catalina 10.15, 10.15.1, 10.15.2, 10.15.3

## 配置

* 处理器：Intel Core i5-7200U

* 内存：8GB Samsung DDR4 2133MHz

* 硬盘：Samsung NVMe SSD Controller PM961 256GB

* 集成显卡：Intel Graphics HD620

* 声卡：Realtek ALC255 with layout-id 30

* 无线网卡：Intel Wireless AC8265

## 不支持的组件

* nVidia MX150

* 指纹传感器

* Intel无线

## 更新记录

2019-07-11:

* 更新VoodooI2C到最新版2.2. 经过两天使用后基本确认没有问题。

2019-07-07:

* 更新Clover到4979
* 更新 Lilu/WhateverGreen/AppleALC/VirtualSMC/NoTouchID 
* 支持Catalina
* 增加RtWlanU驱动
* 移除导致Catalina内核崩溃的`SSDT-PNLF.aml`。同时导致亮度控制不可用

2019-07-19:

* 从macOS Catalina Beta 3 更新到 Beta 4

    * 可直接使用macOS的更新功能升级

    * 更新后不需要重建kext缓存，触摸板正常

    * HiDPI失效，重新执行一遍脚本即可。原因是/System只读，所以更新会直接使用原版进行覆盖

    * 其他正常

2019-08-05:

* 从macOS Catalina Beta 4 更新到 Beta 5

    * 可直接使用macOS的更新功能升级

    * 更新后不需要重建kext缓存，触摸板、HiDPI正常

2019-09-10:

* 从macOS Catalina Beta 5 更新到 Beta 7
* 更新Clover到v5070

2019-09-12:

* 更新到Beta 8

2019-09-24:

* 更新到Beta 9

* 修复了亮度控制

2019-10-01:

* 更新到Beta 10

2019-10-04:

* 更新到Beta 11

2019-10-08:

* 更新到10.15正式版。需要重新启用HiDPI

2019-10-16:

* 10.15补充更新

2019-10-31:

* 更新到10.15.1
* 修改了USB端口限制补丁的MatchOS为10.15.x

2019-12-16:

* 更新到10.15.2

2020-03-29:

* 支持Intel蓝牙

## Credits

- [Acidanthera](https://github.com/acidanthera) for providing [AppleALC](https://github.com/acidanthera/AppleALC), [Lilu](https://github.com/acidanthera/Lilu), [VirtualSMC](https://github.com/acidanthera/VirtualSMC), [VoodooPS2](https://github.com/acidanthera/VoodooPS2), and [WhateverGreen](https://github.com/acidanthera/WhateverGreen).
- [alexandred](https://github.com/alexandred) for providing [VoodooI2C](https://github.com/alexandred/VoodooI2C).
- [apianti](https://sourceforge.net/u/apianti), [blackosx](https://sourceforge.net/u/blackosx), [blusseau](https://sourceforge.net/u/blusseau), [dmazar](https://sourceforge.net/u/dmazar), and [slice2009](https://sourceforge.net/u/slice2009) for providing [Clover](https://sourceforge.net/projects/cloverefiboot).
- [RehabMan](https://github.com/RehabMan) for providing [EAPD-Codec-Commander](https://github.com/RehabMan/EAPD-Codec-Commander) and [OS-X-Clover-Laptop-Config](https://github.com/RehabMan/OS-X-Clover-Laptop-Config).
- [zxystd](https://github.com/zxystd) for providing [IntelBluetoothFirmware](https://github.com/zxystd/IntelBluetoothFirmware).

# Donation

If this project help you reduce time to hackintosh, you can give me a cup of coffee :)

| Wechat| Alipay | PayPal |
| - | - | - |
| ![wechat](img/wechat.png) | ![alipay](img/alipay.png) | [![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=XY2PW7DUBTWXE&source=url) |


