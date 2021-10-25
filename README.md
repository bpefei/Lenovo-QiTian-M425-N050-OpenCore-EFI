## 电脑配置
|配置|型号|
|----|----|
|系统|macOS Big Sur 11.6|
|CPU|Intel Core i5-9400|
|主板|联想313A (B360芯片组)|
|内存|记忆科技 DDR4 2666MHz 8GB|
|硬盘|西数 WDC WD10EZEX-08WN4A0 (1 TB)|
|显卡|Intel UHD Graphics 630 (128 MB / 联想)|
|声卡|Realtek ALC662|
|网卡|Realtek RTL8168/8111/8112 Gigabit Ethernet Controller / 联想|




本机BIOS里没有CFG Lock的关闭选项，请自行搜索教程关闭CFG Lock

经过不断升级，本EFI目前已经升级到OpenCore 0.7.4版本（2021-10-25）。能够支持Big Sur系列最新的系统版本11.6，以上列出的所有硬件均能正常驱动使用，且定制了USB驱动，机箱前后面板的USB接口全部可用。

本EFI升级过程中的历史版本保留在此处。

|     文件夹名     |                             解释                             |
| :--------------: | :----------------------------------------------------------: |
|      EFI-66      | 最初版本，OpenCore 0.6.6。其实只是在“macOS Big Sur 11.2 20D64 Installer for OpenCore 0.6.6 and WEPE”镜像自带的EFI上添加了网卡和声卡支持 |
|      EFI-74      | 和EFI-66配置完全相同，但是OpenCore升级到了0.7.4版，添加了引导界面主题“赛博朋克” |
| EFI-74-Customize | 定制了USB驱动，使用定制的USBPort.kext替换了USBInjectAll.kext，并且在config.plist中作了相应修改。 |
|    EFI-latest    | 定制了核显（UHD 630）驱动，可以60帧输出了，且系统各种缩放动画不再卡顿 |

如果使用最新的EFI不能完成黑苹果安装的话，不妨降低系统版本到macOS Big Sur 11.2，并尝试更旧的EFI版本……

