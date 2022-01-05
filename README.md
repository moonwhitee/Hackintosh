## 简介

这是一份适用于 Opencore P65xHP 的 Hackintosh EFI 配置，机型为 HASEE Z7-Pro。

建议使用[黑果小兵](https://blog.daliansky.net/)镜像，链接就不放了，官网有。
之前有大佬用clover从10.12配置到10.14，我发个10.15.7的（10.15其他版本没试过）
[链接](https://github.com/ConnersHua/Clevo-P65xHP-Hackintosh)

## 说明

### 硬件

机器配置：

- 处理器：英特尔 Core i7-7700HQ @ 2.80GHz 四核
- 主板：Notebook P65xHP（100 Series/C230 Series 芯片组 Family - A152）
- 显卡：Nvidia GeForce GTX 1060 ( 6 GB / 蓝天(CLEVO) )
- 显示器：京东方 BOE0679 ( 15.5 英寸  )
- 以太网卡：Realtek PCIe GbE Family Controller
- 无线网卡：Intel(R) Wi-Fi 6 AX200 160MHz
- 声卡：瑞昱 ALC892 @ 英特尔 High Definition Audio 控制器 （layout-id=15）
- 硬盘：建兴  CV6-8Q128 (固态硬盘)

**关于显卡**

由于神舟战神Z7-pro为独显直连HDMI，而nvidia也仅支持到10.13.6，所以想驱动nvidia只能苟在10.13.6

**关于声卡**

layout-id=15

**关于蓝牙**

已驱动

## 已知问题

- HDMI 无法使用（应该是需要独显，但是 macOS Mojave 10.14.1 开始无法驱动 N 卡），独显直连hdmi无法外接显示器
- 拔掉电源后有可能出现暂时的声卡失效，稍等片刻或接回电源再拔出可解决