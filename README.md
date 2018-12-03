# AiwacProject
These are some PCB project about AIWAC company.
## S905D_MIC
1. 4麦的阵列。
2. 目前没有在研发，资料在网盘。
3. 有两个版本，目前保留第二个版本
## CC3200
1. wiFi模块
2. 资料在网盘
3. 公司没有进行研发
## CC3200
1. AC6901 蓝牙带音频方案，暂时只买了开发板，软硬件暂时还没做开发。
2. 资料在网盘
## DA14580 蓝牙方案
1. 准备做类似米萌尿尿贴产品上，目前原理图和PCB在整理中.
2. 此项目会生产3片小的PCBA，期中触摸板及方案板会功能会跟米萌一致.
3. 新增一个倾斜传感器，放到纸尿裤内进行生产.
4. 这个项目正在做.
## A33_Board_LCD_USB
1. 增加了USB_HUB
2. 增加了LCD屏功能。
3. 触摸模块：可以直接接USB
### 问题1 ：LCD驱动板显示会有水印
1. 初步原因：（1）座子没焊好；（2）或者是LAYOUT的问题；
2. 解决方案：直接买180的LCD屏+驱动板+触摸板，测试过是没有问题。
3. 调试方案：对比资料中的LAYOUT层
### 问题2 ：USB Hub-->带不动USB屏幕
1. 初步原因：初步确定是电流的原因，带不动
2. 解决方案：（1）去掉USB HUB，
3. 调试方案： 拆掉一个芯片，把那一对差分信号直接飞线到那个单独的USB座子
### 总体进度
1. 软件驱动方面，感觉唐元基本调ok了，触摸屏也正常了。
2. wifi,蓝牙，camera，sd卡，串口，声音，电池充电供电，按键开机，开机led灯均正常。
3. 只有usb hub转出来的3个usb口有问题，开始考虑的是如果camera，触摸屏都可能要用usb口，接触摸传感器要用usb口，才需要用usb hub,如果实在不行，可直接将核心板上的usb接口正出来验证下，后面再打一版。
4. 这版现在这样子，建议在上面进一步做量产软件验证。
### 样品生产
1. 基于目前测试好的5套A33底板；
2. 购买OV5640摄像头，回来后焊接成CSI模块
3. 购买MIC，回来后焊接上接插件
4. 购买LCD屏，回来后直接组装
### 采购
| Order | package | number | total price |Link|
| :---: | :-----: | :----: |  :----: |:--:|
|1|HDF 5640-AQ 摄像头--配上连接座 | 4 |  |[深圳市国航芯科电子 6% ](https://item.taobao.com/item.htm?spm=a1z10.3-c-s.w4002-16886023609.16.67b55eddaYQpcq&id=563285697358)
|2|MIC|20||[凯悦电子直销部](https://item.taobao.com/item.htm?spm=a230r.1.14.32.a7f52782W8YtYM&id=561132245409&ns=1&abbucket=18#detail)
|3|LVDS_LCD 屏|4||[锐尔威视](https://item.taobao.com/item.htm?spm=a1z09.2.0.0.47412e8dcDSi7m&id=565149242790&_u=u86c4nsd319)
|4|2500电池 ZH2.54反向插[蓝色套装]----配上连接座|5||[电池](https://item.taobao.com/item.htm?spm=a1z10.1-c-s.w137644-14907183885.20.6cfd356bfhkgXQ&id=41942218237)
|5|喇叭 2840--大小|5||[国创](https://item.taobao.com/item.htm?id=541823569650&tracelogww=ltckbburl)
|6|SH1.0MM端子线 20cm 2P|10||[SH1.0MM端子线 ](https://detail.tmall.com/item.htm?spm=a230r.1.14.6.6fff5e4ax88Mlt&id=552443539764&cm_id=140105335569ed55e27b&abbucket=11&skuId=3991875939611)