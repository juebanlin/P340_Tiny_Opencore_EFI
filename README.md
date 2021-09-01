# OpenCore on P340 Tiny

## 版本
Bigsur,11.5,20g71  

## 硬件配置
-   电源: 230W
-   CPU: Intel Comet Lake i9-10900
-   Chipset: Intel Q470
-   iGPU: UHD 630
-   dGPU: AMD RX560
-   Memory: 16G DDR4 3200 * 2
-   SSD1: 970 PRO PCI-E M.2 512GB (mac)
-   SSD2: 970 EVO PLUS PCI-E M.2 256GB (win10)
-   Sound: ALC235
-   Ethernet: Intel I219-LM7
-   WIFI-M2: [BCM94360CS2 M.2](https://dortania.github.io/Wireless-Buyers-Guide/types-of-wireless-card/m2.html) -> [Windows驱动](./tools/Broadcom_BCM94360CS_Driver_Win_78_10.zip)
-   SMBIOS type iMac20,2

## 完善度
|功能|状态|
|----|---|
|HWP                | ok |
|Sleep              | ok |
|iGPU with HiDPI    | ok |
|Ethernet           | ok |
|WiFi               | ok |
|Bluetooth          | ok |
|USB端口定制         | ok |
|核显独显DP音频输出    | ok |
|Sound              | layout-id=11(0B000000)|



BIOS 设置

1.Devices->ATA Drive Setup->Configure SATA as AHCI

2.Devices->Video Setup->Select Active Video:自动(默认独显输出)

3.Security->Secure Boot->Secure Boot ->Disable  


## 1.下载后请修改序列号
## 2.如果DP没有音频输出则重新插下DP接口