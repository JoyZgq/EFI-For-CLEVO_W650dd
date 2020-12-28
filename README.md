# EFI-For-CLEVO_W650dd

clover v5127，适用于蓝天W650dc，蓝天W650dd（炫龙dc、炫龙dd等）的黑苹果EFI，支持Big Sur

##### 系统版本

![](https://ftp.bmp.ovh/imgs/2020/11/186300ee22e434b4.png)

###### 硬件参数以及对应补丁

| 型号     | 炫龙毁灭着dd | W650dd-dc                |
| ------ | ------- | ------------------------ |
| CPU    | I3-8100 | 免驱                       |
| 集显     | UHD630  | 免驱                       |
| 独显     | GTX960M | 已屏蔽                      |
| 声卡     | ALC269  | 注入ID 58（可修改其他可用点）        |
| WIFI蓝牙 | Intel   | 使用AirportItlwm实现         |
| USB    | 2.0/3.0 | USBPorts.kext            |
| 键盘     |         | VoodooPS2Controller.kext |

### 尚待解决的问题

- [ ] 显卡存修复1536M--->2048MB

- [ ] 亮度调节补丁Fn+F8，Fn+F9,网上有相关帖子[使用SSDT 给 CPU 变频 及 X86PlatformPlugin 小教程-思羽布丁](https://www.mfpud.com/topics/963/)，目前采用[QuickShade](https://apps.apple.com/cn/app/quickshade/id931571202)第三方工具，可以自定义

- [x] ~~关于Wi-Fi驱动有两种方式一个是itlwm+HeliPort，另一个是AirportItlwm.kext,前者需要使用HeliPort，推荐设为开机启动，后者功能更多（似乎可以实现隔空投送）但目前是beta版，在10.15.7上测试是对比前者速度较快，但在bigsur会出现Wi-Fi无法正常使用，CPU居高不下的问题，以后出现稳定版会继续测试~~

附带

[黑苹果:主板解锁CFG LOCK教程 - 哔哩哔哩](https://www.bilibili.com/read/cv6167464/)

有问题欢迎讨论

参考：

 [[**CLOVER**]](http://bbs.pcbeta.com/forum.php?mod=forumdisplay&fid=561&filter=typeid&typeid=1366) [2020.9.25 炫龙DC (DD)(Pro)神舟K670(K680) 蓝天W650 10.15.7 clover5122](http://bbs.pcbeta.com/viewthread-1831835-1-1.html)
