## 电脑配置
|配置|型号|
|----|----|
|系统|macOS Big Sur 11.2|
|CPU|Intel Core i5-9400|
|主板|联想313A (B360芯片组)|
|内存|记忆科技 DDR4 2666MHz 8GB|
|硬盘|西数 WDC WD10EZEX-08WN4A0 (1 TB)|
|显卡|Intel UHD Graphics 630 (128 MB / 联想)|
|声卡|Realtek ALC662|
|网卡|Realtek RTL8168/8111/8112 Gigabit Ethernet Controller / 联想|




本机BIOS里没有CFG Lock的关闭选项，请自行搜索教程关闭CFG Lock

EFI文件夹是OpenCore 0.6.6版本的，EFI74-with-theme文件夹是升级到目前最新版0.7.4版本的，还加了个"赛博朋克"主题。

Customize/USBPorts.kext是定制好的USB驱动，如果需要升级到11.3版本以上，请使用USBPorts.kext替换EFI/OC/Kexts目录下的USBInjectAll.kext，并且使用Customize/config.plist替换EFI/OC目录下的config.plist（注意：Customize/config.plist是0.7.4版本的OpenCore配置文件，所以请搭配EFI74文件夹使用）
