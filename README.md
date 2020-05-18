# ASRock-Z390M-ITX-ac-OpenCore
ASRock-Z390M-ITX/ac OpenCore config files for hackintosh.

华擎 Z390M ITX/ac 黑苹果 OC 配置文件

Based on https://dortania.github.io/OpenCore-Desktop-Guide/

根据 https://dortania.github.io/OpenCore-Desktop-Guide/ 配置而来
[![YfAGFA.md.jpg](https://s1.ax1x.com/2020/05/18/YfAGFA.md.jpg)](https://imgchr.com/i/YfAGFA)
[![YfAxTH.png](https://s1.ax1x.com/2020/05/18/YfAxTH.png)](https://imgchr.com/i/YfAxTH)
[![YfEPpt.png](https://s1.ax1x.com/2020/05/18/YfEPpt.png)](https://imgchr.com/i/YfEPpt)
## Hardwares
- CPU: Intel I5 9600KF
- Motherboard: ASRock Z390M ITX/ac, with Dual NIC.
- Graphics card: PULSE RX 580 8G G5
- Wifi Card: BCM94360CS2

## 配置
- CPU：Intel I5 9600KF
- 主板：华擎 Z390M ITX/ac, 双网卡
- 显卡：蓝宝石 RX580 白金版（2304SP）
- 无线网卡：BCM94360CS2

## What Works
- Aridrop and handoff
- Intel I211AT with SmallTreeIntel82576
- Intel I219V with IntelMausiEthernet.kext
- USB Ports
- Audio
- NVRAM with SSDT-PMC.aml
- Sleep and Wake

## 正常工作
- 双有线网卡
- wifi，蓝牙
- 隔空投送、接力
- 睡眠与唤醒
- 声音
- USB（由于我的 ITX 机箱没有前置 USB 面板，所以目前定制的版本，15个端口全部使用的主板 IO 面板上的）


## Version Infos 版本信息
| item                | version |
| ------------------- | ------- |
| OpenCorePkg         | 0.5.8   |
| Lilu                | 1.4.4   |
| AppleALC            | 1.4.9   |
| VirtualSMC          | 1.1.3   |
| WhateverGreen       | 1.3.9   |
| IntelMausi          | 1.0.2   |
| SmallTreeIntel82576 | unknow  |


## 安装注意
1. 先按照[推荐配置](https://dortania.github.io/OpenCore-Desktop-Guide/config.plist/coffee-lake.html#intel-bios-settings)修改自己的主板 BIOS, 找不到的选项可以忽略
2. 推荐使用[黑果小兵](https://blog.daliansky.net/)的镜像，用 Etcher 写入 U 盘，然后将本项目的内容放到 U盘 EFI 分区的 EFI 文件夹中，从 boot/BOOTX64.efi 启动
3. 你需要设置你自己的SMBIOS信息，参考[这里](https://dortania.github.io/OpenCore-Desktop-Guide/config.plist/coffee-lake.html#platforminfo)
4. https://dortania.github.io/OpenCore-Desktop-Guide 这个指南真的很全面，大部分问题你都可以找到解决方案。尤其是其中的 TROUBLESHOOTING 章节。