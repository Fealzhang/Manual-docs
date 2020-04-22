



![herelink20200422](assets/herelink20200422.png)















# 概述

Herelink是一款集遥控器、地面站、视频和数传的高度集成系统，可与Cube Autopilot、ArduPilot或PX4使用。

Herelink最大传输可达20公里的RC控制、高清视频和遥测数据，Herelink遥控器采用Solex TX和QGC开源地面站。





# 特点

- 基于Android的智能设备配有5.46英寸的1080p LCD触摸屏。
- 集视频、遥测、控制于一体的数字传输系统。
- Solex TX和QGC地面站软件与mavlink支持ArduPilot和PX4。
- 使用双回中霍尔摇杆，上端摇杆可支持拆卸更换。
- 1080p高清视频与双数字视频输入。
- 双S.bus信号输出，可同时控制自动驾驶仪和云台相机。
- 6 个自定义按键和 1个滚轮。
- 独立于Solex TX / QGC的专用RC云台信号控制。 
- 通过WIFI或局域网连接实现地面站遥测信息和视频共享。





# 硬件参数

## 技术规格

**天空端与地面端硬件信息：**

- 处理器：SoC – 澎湃 S1

- AP：4 x 大核 , Cortex A53, 2.2GHz

​       4 x 小核 , Cortex A53, 1.4GHz

- GPU：4 核, Mali-T860
- SDR：A7 + DSP
- 存储：天空端 LPDDR3 1GB , 地面端 LPDDR3 2GB
- 天空端 / 地面端：EMMC: 4GB
- 图传距离：FCC 20km   CE / SRRC / MIC 12km
- 图传延时：最小 110 ms
- 图传像素：720p@30fps 1080p@30/60fps
- 传输频段：2.4GHz ISM
- 接收灵敏度：-99dBm@20MHz BW
- 干扰恢复：< 1s

------



- ##### 天空端：

  
  
  ![herelink](Z:\Herelink产品资料\HereLink数图传\herelink.png)





- 壳体：铝合金
- 重量：95g（含天线）
- 尺寸：78.5×30×15mm
- 信号带宽：20MHz / 10MHz
- 功耗：图传模组单侧平均功耗小于 4 W
- Micro HDMI 1： 用于外部相机视频信号输入（首选）
- Micro HDMI 2： 用于外部相机视频信号输入
- Power 接口：5V - 12.6V 电源输入接口
- UART 接口：3.3V / 5V 电平UART接口
- S.bus 接口：两条 RC 输出接口，S.bus1和S.bus2
- Micro USB：用于调试升级，支持 OTG 模式
- 按键孔：用于对频及状态重置
- 指示灯 1 ，2：用于指示对频和图传状态
- MMCX 天线插口 1，2：用于数图传信号与地面通信

------



- ##### 地面端：

  ![黑白轮廓图](../../../../9-27%E6%88%AA%E8%87%B3%E6%8A%80%E6%9C%AF%E6%96%87%E6%A1%A3%E6%95%B4%E7%90%86/Carrey/%E8%AF%B4%E6%98%8E%E4%B9%A6/assets/%E9%BB%91%E7%99%BD%E8%BD%AE%E5%BB%93%E5%9B%BE.png)

- 壳体：塑胶
- 重量：516g（含天线）
- 尺寸：217×106.5×31mm (整机不含外置天线和摇杆)
- 屏幕 ：5.46 寸，1080P，1600 万色，电容式触摸屏
- 音频 ：内置扬声器 *1，内置麦克风 *2
- 遥控 ：摇杆 *2 ，滚轮 *1 ，底部按键 *6  有背光，顶部按键 *1（右）
- 通信 ：WIFI / GPS   2.4GHz 图传地面端
- 指示灯：顶部三色灯 *2（左，右）
- 接口 ：MicroUSB *1 ，Tflash *1（支持最大 64GB 扩展）
- 天线 ：定向(5dBi) *1 可拆卸 ，全向(2dBi) *1 可拆卸 
- 内置 wifi 天线 ，内置 GPS 天线 ，外置 GPS 天线接口
- 电源 ：内置 4950 mAh Lipo Battery
- 充电 ：支持 Micro USB 口 5V 2A 电流充电
- 功耗：平均功耗不超过 4W（仅图传工作，屏幕亮度中等，WiFi 关闭，GPS 关闭）





## 产品配件

1. HereLink天空端 *1
2. HereLink遥控端 *1
3. 遥控端全向天线 *1
4. 遥控端定向天线 *1
5. 天空端天线 *2
6. 遥控端摇杆 *2
7. HDMI线 *1
8. 电源线 *1
9. 数传线 *1
10. S.bus线 *1
11. USB线 *1
12. 背板 *1
13. M1.6，16mm（散热扇螺丝）*5
14. M1.6（散热扇螺母）*5
15. 垫片（散热扇垫片）*5
16. 硅胶圈（散热扇用）*20
17. M1.6，3mm（天空端背板固定螺丝）*5
18. M3，10mm（背板固定螺丝）*3
19. M3螺母（背板固定螺母）*3

`*风扇不在Herelink标配内，并且正常情境下非必需`





## 接口定义

- ##### 天空端：                   

  ​                                                                                                           

![天空端侧面接口图123](Z:\Herelink产品资料\HereLink数图传\天空端侧面接口图.png)





![123](Z:\Herelink产品资料\HereLink数图传\飞控接口.png)





**Power：**

| Pin # | Name  | Description                             |
| ----- | ----- | :-------------------------------------- |
| 1     | Power | Power IN，5V - 12.6V max（支持3s Lipo） |
| 2     | GND   | Ground pin                              |



**UART：**

| Pin # | Name | Description                     |
| ----- | ---- | ------------------------------- |
| 1     | RXD  | RX of air module，3.3V / 5V TTL |
| 2     | TXD  | TX of air module，3.3V / 5V TTL |
| 3     | GND  | Ground pin                      |



**S.bus ：**

| Pin # | Name        | Description    |
| ----- | ----------- | -------------- |
| 1     | S.bus out 1 | 遥控器信号输出 |
| 2     | GND         | Ground pin     |
| 3     | S.bus out 2 | 云台控制       |
| 4     | GND         | Ground pin     |





## 天空端状态指示灯

**LED1：**

绿灯常亮  接收到 HDMI 1 视频信号

红灯常亮  接收到 HDMI 2 视频信号

黄灯常亮  接收到飞控信号

绿灯红灯交替闪烁  接收到两路视频信号

绿灯黄灯红灯交替闪烁  接收到两路视频信号以及飞控信号

灯不亮  未接收到有效视频 / 飞控信号        



**LED2：**

绿灯闪烁  对频进行中

绿灯常亮  电源正常且接收到有效信号

黄灯常亮  未对频 / 未接收任何有效信号

红灯闪烁  电源不稳定

灯不亮  天空端未接电



**Pair / Reset 键：**

遥控器对码及进入升级模式





## 遥控端按键及指示灯

**按键：**

左上方滚轮：控制云台

右上方按键：拍照按键（可自定义通道按键）

下方按键A : 可自定义通道按键

下方按键B：可自定义通道按键

下方开关机键：开关机与解锁屏键

下方HOME键：可自定义通道按键

下方按键C：可自定义通道按键

下方按键D：可自定义通道按键



**指示灯（左）：**

红灯闪烁：电量较低

红灯常亮：电量不足

黄色常亮：电量中等

绿色常亮：电量充足





# 固件更新

**下载更新固件应用程序：**

- Windows端：https://herelinkfw.cubepilot.org/flasher_win.zip
- MAC端：https://herelinkfw.cubepilot.org/flasher_mac.zip
- Linux端：https://herelinkfw.cubepilot.org/flasher_linux.zip

1. 通过USB将Herelink遥控器连接到PC。
2. 遥控器开机时同时按**电源**和**D**按键，将Herelink遥控器启动到Fastboot中。
3. 解缩并运行应用程序，双击打开应用程序会自动开始刷写，等待刷写完成会自动重启。
4. 将Herelink天空端供**5-12v**电源，然后通过USB将Herelink天空端连接到PC。
5. 双击打开应用程序会自动开始刷写，等待刷写完成会自动重启。
6. Herelink设备将通过“激活”窗口启动，请按照以下步骤继续操作。

`请注意：在安装有Solex TX应用程序的较新固件版本中，可以通过wifi网络更新Herelink遥控器固件。`



# Herelink设备激活

升级Herelink固件后，需要激活设备，屏幕将显示“更新设备”。

**注意：Herelink必须通过WiFi连接到互联网，才能激活。**

- 从设置菜单将Herelink连接到您的WiFi连接。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M4EOp4veR8IIl55wW5n%2F-M4EOpwN43sxWAOEdC3Y%2Factivation1.jpg?generation=1586175112766520&alt=media)



- 右上角选择您的地区，然后点击“继续”。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M4EOp4veR8IIl55wW5n%2F-M4EOpwPOrc-szIPMpL8%2Factivation3.jpg?generation=1586175121636005&alt=media)



- 然后将提示您输入您的16位软件激活密钥。 

**注意：在更高版本的Herelink版本中，您的密钥将位于包装盒上，对于早期的Herelink版本，您应与原始经销商联系以获得有效的许可密钥。**

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M4EOp4veR8IIl55wW5n%2F-M4EOpwRcwpEfpG6blJk%2Factivation2.jpg?generation=1586175115469618&alt=media)

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M4EOp4veR8IIl55wW5n%2F-M4EOpwTbdD8tPVoY7Q7%2Factivation4.jpg?generation=1586175116039994&alt=media)

- 输入后，点击“完成”，然后再点击“注册”，您的设备将下载最新固件程序并自动更新安装。





# **通过WiFi进行固件更新**

如果您的Herelink固件是已安装Solex TX，则可以通过内置的更新功能来更新地面站。

**注意：Herelink天空端仍然需要使用PC端更新程序来更新。**

- 确保您将Herelink遥控器连接到wifi并且有网络。
- 从顶部下拉并在右上角选择设置齿轮 。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M2lI7HZGVY2STNo0O9R%2F-M2lI8Ks7z3rERb6bfg3%2Fsettings-1.jpg?generation=1584596305163342&alt=media)




- 滑动到底部，然后点击“关于手机”选项。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M2lI7HZGVY2STNo0O9R%2F-M2lI8Kuf65psbi2MXTZ%2Fsettings.jpg?generation=1584596307154764&alt=media)



- 选择“系统更新” 。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M2lI7HZGVY2STNo0O9R%2F-M2lI8KwkcvEmLCwO0of%2Fsystem-update.jpg?generation=1584596304192453&alt=media)



- 选择右下角的“检查更新”。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M2lI7HZGVY2STNo0O9R%2F-M2lI8Kyif7LghDrUGbh%2Fupdate.jpg?generation=1584596306350902&alt=media)



- 系统将检查更新并自动安装。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M2lI7HZGVY2STNo0O9R%2F-M2lI8L-agxjAHOuAhDv%2Fupdating.png?generation=1584596303613035&alt=media)



> **如果Herelink远程更新错误，请检查以下三步**
>
> 1. 是否已连接到稳定有网络的wifi 
> 2. 设备的时间是否正确
> 3. 输入的密钥是否正确





# 遥控器摇杆校准

- 在应用程序界面中，从顶部向下滑动通知栏，然后选择Herelink Setting。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M2lI7HZGVY2STNo0O9R%2F-M2lIA24M1LTijhx_PGS%2Fhome-screen.png?generation=1584596325426029&alt=media)

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M2lI7HZGVY2STNo0O9R%2F-M2lIA26pebAjL0dG_Tt%2Fsettings-app.jpg?generation=1584596326121287&alt=media)



- 向左滑动以显示摇杆校准界面。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M021ptM_ijH8Yxy-JuC%2F-M025fTfwFaNyutNsvwh%2Fdevice-2020-02-14-151909.png?alt=media&token=52e765e5-cb6d-4e78-a304-a5f3520e7f00)



- 要校准滚轮，请选择“ HW WHEEL CAL”。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M2lI7HZGVY2STNo0O9R%2F-M2lIA28JfRHcZdR-9jr%2Fhw-wheel-2.jpg?generation=1584596326801442&alt=media)



- 点击“开始滚轮校准”，然后按提示进行校准。

- 完成后，点击“通过”返回。

![39](Z:\Herelink产品资料\HereLink数图传\图片新\39.png)

![40](Z:\Herelink产品资料\HereLink数图传\图片新\40.png)



- 要校准硬件摇杆，请单击“ HW JS CAL”。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M2lI7HZGVY2STNo0O9R%2F-M2lIA2CeN6esYzqT3_w%2Fjoystick.jpg?generation=1584596324790069&alt=media)



- 摇杆校准，点击开始校准，根据摇杆箭头与右侧提示进行硬件摇杆校准。

![43](Z:\Herelink产品资料\HereLink数图传\图片新\43.png)

![41](Z:\Herelink产品资料\HereLink数图传\图片新\41.png)



- 摇杆校准完成后。会提示检测通过，点击下面通过按钮即完成硬件摇杆校准，如果校准过程中出现问题或校准失败，请重新校准。

![42](Z:\Herelink产品资料\HereLink数图传\图片新\42.png)



- 校准遥控SBUS，请单击“ SBUS OUT CAL”，然后按照突出显示部分中显示的步骤进行操作。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M2lI7HZGVY2STNo0O9R%2F-M2lIA2IxxNJdcnnYWET%2Fjoystick-sbus.jpg?generation=1584596326312079&alt=media)

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M4EOp4veR8IIl55wW5n%2F-M4EOqA7FwOPD33XubMV%2Fcalibrate2.png?generation=1586175120910364&alt=media)

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M4EOp4veR8IIl55wW5n%2F-M4EOqA9h9MQnbCbzgu7%2Fcalibrate1.png?generation=1586175118877111&alt=media)





# 与天空端对频

- 通过下滑通知栏并点击Herelink Settings来打开设置。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M2lI7HZGVY2STNo0O9R%2F-M2lIA26pebAjL0dG_Tt%2Fsettings-app.jpg?generation=1584596326121287&alt=media)



- 点击“pair”按钮，然后按住天空端上的Pair/Reset按钮直到LED2指示灯闪烁。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M4EOp4veR8IIl55wW5n%2F-M4EOqABh_LHyAA7xx5R%2Fsettings101.png?generation=1586175119835114&alt=media)

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M4EOp4veR8IIl55wW5n%2F-M4EOqADLGgj88RUvIdU%2Fairpair1.png?generation=1586175115933319&alt=media)

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M4EOp4veR8IIl55wW5n%2F-M4EOqAFJdEJUhCsuGUF%2Fairpair2.png?generation=1586175116932299&alt=media)





# 功率模式设置

- 从此处设置你所在国家/地区所符合的功率发射模式。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M4EOp4veR8IIl55wW5n%2F-M4EOqAH0OQ-aWbPEAH2%2Ffccsettings.png?generation=1586175117914003&alt=media)





# 按键和滚轮设置

**在Solex TX中配置按键**：

- 打开Solex TX App 。
- 单击左上角的菜单栏。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M2lI7HZGVY2STNo0O9R%2F-M2lI8_C96WVrtnSzbSq%2Fbutton-mapping-0.jpg?generation=1584596319321998&alt=media)



- 选择“按键映射” 。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M2lI7HZGVY2STNo0O9R%2F-M2lI8_FQjWZX-RdWUaK%2Fbutton-mapping-1.jpg?generation=1584596320244322&alt=media)



- 选择需要设置的按键。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M2lI7HZGVY2STNo0O9R%2F-M2lI8_HNsnfYL7iz0ES%2Fbutton-mapping-2.jpg?generation=1584596318201846&alt=media)



- 选择“短按(On Click)” 或 “长按(On long click)”（**请注意，**这允许您为每个按键设置两个功能）。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M2lI7HZGVY2STNo0O9R%2F-M2lI8_JRkxbXUTYeCgv%2Fbutton-mapping-2.5.jpg?generation=1584596314113839&alt=media)



- 例如想使用A按键控制所需功能，点击Button A,然后点击右侧选项框选择所需功能。


![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M2lI7HZGVY2STNo0O9R%2F-M2lI8_LSWBLKUAL8hpS%2Fbutton-mapping-3.png?generation=1584596312277749&alt=media)



- 示例功能为飞行模式，选择功能后点击旁边的小齿轮设置选择需要的飞行模式。


![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M2lI7HZGVY2STNo0O9R%2F-M2lI8_NOGWqZ2ttqJBY%2Fbutton-mapping-6.jpg?generation=1584596308121240&alt=media)



- 选择飞行模式。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M2lI7HZGVY2STNo0O9R%2F-M2lI8_PkGdkL0WPJHNz%2Fbutton-mapping-5.png?generation=1584596309717591&alt=media)



- 其它需要设置的按键，按以上按键设置重复操作并选择对应功能，然后点击底部的“SAVE BUTTONS”保存。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M2lI7HZGVY2STNo0O9R%2F-M2lI8_RYTqvHH43fw3r%2Fbutton-mapping-7.jpg?generation=1584596316175312&alt=media)



**在QGC中配置按键**：

- 打开QGC。
- 点击左上角的小齿轮设置选择。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M2lI7HZGVY2STNo0O9R%2F-M2lI8_TGw7xN5TUWLUu%2Fqgc-button-1.jpg?generation=1584596322134270&alt=media)



- 选择“Buttons” 按键选项框。
- 勾选左侧所需按键的框。
- 点击下拉菜单选择功能。
- 对每个按键重复操作并选择需要使用的飞行模式。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M2lI7HZGVY2STNo0O9R%2F-M2lI8_VSBZllFgCQXfc%2Fscreenshot-2020-03-16-at-22.35.57.png?generation=1584596323270305&alt=media)





**滚轮设置**：

左上角滚轮默认映射到SBUS通道5。也可以在Solex TX中将其配置为飞控上的1-16输出通道，也可以通过Solex TX中的按键设置切换滚轮的控制通道。



- 打开Solex TX App 。
- 单击左上角小3行的菜单选项。
- 选择“Button Mapping”。
- 点击右下角的“WHEEL SETTINGS”滚轮设置。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M2lI7HZGVY2STNo0O9R%2F-M2lI8_XrUsbaZm4LI1N%2Fwheel-1.jpg?generation=1584596311172400&alt=media)


- 从1到16中选择所需的伺服通道。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M2lI7HZGVY2STNo0O9R%2F-M2lI8_ZclEbK8HCdI-c%2Fwheel-2.jpg?generation=1584596313240178&alt=media)



- 设置适合您应用的PWM输出范围。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M2lI7HZGVY2STNo0O9R%2F-M2lI8_aKWmzYvo4hqpv%2Fwheel-4.jpg?generation=1584596315205464&alt=media)



- 点击选上“Enabled”框以激活输出，然后点击“OK”保存。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M2lI7HZGVY2STNo0O9R%2F-M2lI8_c_FDksEJlkde4%2Fwheel-5.png?generation=1584596310237066&alt=media)



- 要切换滚轮控制通道输出，请将一个按键设置为“滚轮设置”。来切换滚轮通道。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M2lI7HZGVY2STNo0O9R%2F-M2lI8_eXDFyJaEvnFbD%2Fwheel-6.jpg?generation=1584596321468979&alt=media)



- 点击右侧的小齿轮设置另一个滚轮切换通道和PWM值，点击OK确定，然后点击底部右侧的“SAVE BUTTONS”保存按键设置。


![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M2lI7HZGVY2STNo0O9R%2F-M2lI8_g7KEE-YJguv5G%2Fwheel-7.png?generation=1584596317241442&alt=media)

- 更改后，滚轮将在新设置的通道上输出，要切换回原来的通道输出，需要将一个按键功能设置为“ Clear Wheel Settings”，来打开和关闭通道进行滚轮通道切换，如上二图所示。





# 视频分享

**在Herelink上启用视频流**：

- 向下滑动通知栏，然后点击“ herelink Settings”。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M2lI7HZGVY2STNo0O9R%2F-M2lIA26pebAjL0dG_Tt%2Fsettings-app.jpg?generation=1584596326121287&alt=media)



- 找到“Video Sharing”并启用视频共享。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M2lI7HZGVY2STNo0O9R%2F-M2lIAKHErvkkZ0ngbiI%2Fvideo-sharing.jpg?generation=1584596327481263&alt=media)

请注意，视频流在GCS应用程序启用之前是不可用的，因此请确保至少有一个GCS应用程序在后台运行，并选择正确的视频流。



**通过wifi热点连接分享视频**：

- 下拉通知栏并启用热点。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M01spuHUvrI3MO4-Rla%2F-M01vyWxKNJzrKeLuJ-j%2Fdevice-2020-02-14-143024.png?alt=media&token=bb6ae3a5-dcc6-468e-aad5-bf9cc63b04a0)



- 要设置请按住热点徽标，将跳转到设置界面。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M01spuHUvrI3MO4-Rla%2F-M01wP5F558fH1eCavZf%2Fdevice-2020-02-14-143404.png?alt=media&token=878ecc79-1699-42b9-8aeb-117ac87f4f9a)



- 然后在“设置WLAN热点”下为该热点配置名称和密码。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M4EOp4veR8IIl55wW5n%2F-M4EOpgO_2F80F1XztX_%2Fpassword.png?generation=1586175111058507&alt=media)

- 视频流的地址为：`rtsp://192.168.43.1:8554/fpv_stream`



**通过USB连接分享视频**：

- 菜单栏下拉，按住热点徽标，跳转到设置界面。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M01spuHUvrI3MO4-Rla%2F-M01vyWxKNJzrKeLuJ-j%2Fdevice-2020-02-14-143024.png?alt=media&token=bb6ae3a5-dcc6-468e-aad5-bf9cc63b04a0)



- 在"网络共享与便携式热点"里找到 USB网络共享，打开它。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M01spuHUvrI3MO4-Rla%2F-M01wP5F558fH1eCavZf%2Fdevice-2020-02-14-143404.png?alt=media&token=878ecc79-1699-42b9-8aeb-117ac87f4f9a)

- 视频流`rtsp://192.168.42.129:8554/fpv_stream`将通过USB连接传输给连接的设备。



**通过Wifi连接分享视频**：

- Herelink通过连接5G Wifi，则可以使用网络上的Herelink IP获得视频流。
- 下滑通知栏，按住“ Wifi”徽标，跳转到Wifi界面，然后点击右侧设置。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M01spuHUvrI3MO4-Rla%2F-M01yNhdtNI7ZKCXvABX%2Fdevice-2020-02-14-144314.png?alt=media&token=68775b2e-63a3-48e9-a04b-73469be24400)



- 向下滑动以找到IP地址。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M01spuHUvrI3MO4-Rla%2F-M01ytG-JTn1qR8sboeX%2Fdevice-2020-02-14-144436.png?alt=media&token=01082abe-cce5-4a11-a081-dbccb31aa527)

- 视频流的连接地址为： `rtsp://<ipaddress>:8554/fpv_stream`



**显示视频流** :

在此示例中，我们使用VLC媒体播放器。

- 打开VLC播放器并点击媒体>>打开网络串流。
- 输入HereLink上提供的IP地址，然后点击“播放” 。

![VCL视频](assets/VCL视频.png)





# 与Mission Planner地面站连接

**使用WiFi热点与地面站连接**：

打开Herelink上的热点，将电脑Wifi连接到Herelink的WiFi热点。

- 打开地面站。
- 将端口设置为“UDP”(右上角)。
- 点击“连接”。
- 输入端口号 “14550”。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-LqzIj9PLZo-wxvbKg28%2F-LqzJ-8wvuSXxIh4zHME%2Fscreen-udp-copie-min.jpg?generation=1570872777696960&alt=media)

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-LqzIj9PLZo-wxvbKg28%2F-LqzJ-8ysVfPuoXIzipd%2Fmission-planner-2.png?generation=1570872769477304&alt=media)



**使用Wifi网络，局域网连接** :

**电脑连接到Herelink所在的Wifi网络，局域网：**

- 打开Mission Planner地面站。
- 将端口设置为“ UDPCL”（右上角）。
- 点击“连接”。
- 输入Herelink的IP地址（遥控器下拉菜单栏-点击右上角的设置-关于手机-状态信息-IP地址）。
- 输入端口号“ 14552”。

现在，Mission Planner地面站也可以使用mavlink遥测数据。



**在Mission Planner中观看实时Herelink视频**：

**注意：视频需要Mission Planner 1.3.70 Beta或更高版本。**

- 启动Solex或QGC以确保您的视频正常工作（这是开始视频传输过程所必需的）。
- 在HUD区域右击。
- 选择“Video” 。
- 选择“Herelink Video”。
- 首次执行此项程序时，可能需要下载播放视频所需的文件。您的设备将需要连接有效的网络才能执行此操作，（您的电脑需要断开Herelink热点才能执行此步骤）。
- 将弹出窗口，输入Herelink的IP地址（遥控器下拉菜单栏-点击右上角的设置-关于手机-状态信息-IP地址），然后点击“确定”。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M2lI7HZGVY2STNo0O9R%2F-M2lI9Zc3CDmOOxYmkLv%2Fherelink-video.jpg?generation=1584596324441027&alt=media)

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M2lI7HZGVY2STNo0O9R%2F-M2lI9ZecuOqYcIp01kG%2Fherelink-video-ip.jpg?generation=1584596324591890&alt=media)





# 安装自定义应用

**确保您已在电脑系统中安装了最新的平台工具**

平台工具地址（需VPN）：https://developer.android.com/studio/releases/platform-tools

- 下拉菜单栏点击右上角设置-关于手机-滑到最底下的版本号-连续点击直至出现开发者模式。
- 打开设置-开发者模式-打开“USB调试”。
- 用USB将Herelink和电脑连接。
- 检查设备是否连接正常。

`$ adb devices`
`List of devices attached`
`66c4bfea    device`



- 安装应用程序： `adb install <app_name>.apk`

`$ adb install myapp.apk`
`Performing Streamed Install`
`Success`



- 应用安装完成后，您的应用程序应该出现在桌面列表中。

![img](https://gblobscdn.gitbook.com/assets%2F-LUhw7cdLeWVORgnTA3i%2F-M021ptM_ijH8Yxy-JuC%2F-M022nY30A8E526xsNcs%2Fdevice-2020-02-14-150633.png?alt=media&token=b17ae03e-0a4a-4828-8ff7-4d03aa15da40)



- 删除应用程序： `adb remove org.myorg.appname`

`$ adb remove org.myorg.appname`
`Success`





# OEM图像设置

**Linux系统**

**必要条件：**

Android工具：https://developer.android.com/studio/releases/platform-tools

**操作步骤：**

- 下载并解压缩以下文件：

- simg2img：https://herelinkfw.cubepilot.org/tools/simg2img_linux.zip
- img2simg：https://herelinkfw.cubepilot.org/tools/img2simg_linux.zip
- 遥控端 oem_ru_base.img：https://herelinkfw.cubepilot.org/tools/oem_ru_base.img
- 天空端 oem_au_base.img：https://herelinkfw.cubepilot.org/tools/oem_au_base.img

- 根据要修改的设备选择映像文件。

- 下载并解压缩到同一个目录中。

- 现在，要从上面下载的稀疏图像(.img)生成ext4fs映像，请执行以下操作：

  `./simg2img_mac oem_au_base.img raw_oem_au_base.img`

- 使用以下命令创建挂载点目录 ：

  `mkdir oem`

- 使用`mount raw_oem_au_base.img oem`挂载映像。

- 现在您应该能够修改挂载目录中的文件了。

- 需要使用`sudo`才能够在挂载文件内操作。

- 完成更改后，需使用以下命令卸载驱动器：

  `sudo umount oem`

- 然后使用命令将ext4fs映像转换回android稀疏图像：

   `./img2simg raw_oem_au_base.img oem_au.img`

- 现在，您可以使用以下命令启动到引导加载程序，将该映像刷写到天空端中 ：

  `adb reboot bootloader`

- 最后运行以下命令：

  `fastboot flash oem oem_au.img`



**MacOS系统**

**必要条件：**

Homebrew工具：https://brew.sh/

Android工具：https://developer.android.com/studio/releases/platform-tools

**操作步骤：**

- 安装osxfuse在您的电脑系统中，使用以下代码安装，这将需要重启您的电脑系统:

  `brew cask install osxfuse`

- 请按照以下网址链接的步骤安装fuse-ext2。这将允许您挂载将要生成的ext4fs。

  https://github.com/alperakcan/fuse-ext2#macos

- 下载并解压缩以下文件：

- simg2img：https://herelinkfw.cubepilot.org/tools/simg2img_mac.zip
- img2simg：https://herelinkfw.cubepilot.org/tools/img2simg_mac.zip
- 遥控端 oem_ru_base.img：https://herelinkfw.cubepilot.org/tools/oem_ru_base.img
- 天空端 oem_au_base.img：https://herelinkfw.cubepilot.org/tools/oem_au_base.img

- 根据要修改的设备选择映像文件。

- 下载并解压缩到同一个目录中。

- 现在，要从上面下载的稀疏图像(.img)生成ext4fs映像，请执行以下操作：

  `./simg2img_mac oem_au_base.img raw_oem_au_base.img`

- 使用以下命令创建挂载点目录 ：

  `mkdir oem`

- 使用`fuse-ext2 raw_oem_au_base.img oem -o rw+`挂载映像。

- 现在您应该能够修改挂载目录中的文件了。

- 需要使用`sudo`才能够在挂载文件内操作。

- 完成更改后，需使用以下命令卸载驱动器：

  `sudo umount oem`

- 然后使用命令将ext4fs映像转换回android稀疏图像：

   `./img2simg raw_oem_au_base.img oem_au.img`

- 现在，您可以使用以下命令启动到引导加载程序，将该映像刷写到天空端中 ：

  `adb reboot bootloader`

- 最后运行以下命令：

  `fastboot flash oem oem_au.img`



**示例：**

- 在以下示例中，我们更改了Herelink天空端板的系统ID。

- 大多数配置文件位于`/system/etc`，下面的例子中，我们将使用命令`adb pull /system/etc/system-control.telepathy-air.conf`来获取配置。

- 获取配置后，文件将包含以下信息：

`# module on/off`

`board_control_enabled = true`

`d2d_tracker_enabled = true`

`camera_control_enabled = true`

`# board control`

`board_system_id = 42`

`# camera control`

`video_stream_ip_address = 192.168.0.10`

`camera_system_id = 42`

`support_multiple_camera = true`

`support_camera_capture = false`

- 您可以在您的编辑器中根据需要更改`board_system_id`和`camera_system_id`字段的值。

- 编辑完成后，保存此文件并退出编辑器。

- 使用命令`sudo mkdir oem/etc`在oem映像中创建一个名为etc的文件夹。

- 使用文件复制命令：`sudo cp system-control.telepathy-air.conf oem/etc/`

- 继续把映像栏卸载然后依上面的描述刷进(天空/地面)端里。





# 生成错误报告

**安装ADB和Google驱动程序**

**下载SDK平台工具和谷歌的USB驱动程序：**

SDK平台工具：https://developer.android.com/studio/releases/platform-tools

谷歌USB驱动程序：https://developer.android.com/studio/run/win-usb



**用ADB设置设备：**

在Herelink设备上启用Developper选项：

- 在主屏幕上，点击Android应用程序菜单（屏幕右下方）。

- 点击进入“设置”>“关于手机” >>“版本号” 。

- 在“版本号”上点击七次，它将激活开发者模式。会弹出消息框，设备现在处于开发者模式。

- 点击左侧的小三角形返回>>进入“开发者选项” >>打开“ USB调试” 。



**生成错误报告：**

- 使用USB线将Herelink遥控器连接到计算机上。

- 打开计算机的终端，然后输入命令:`adb bugreport` >按下回车键，命令将生成bureport日志文件并以.zip文件保存在设备上。

- 使用以下命令将.zip文件发送到您的计算机：

  `adb pull <filepath_of_zip_file_on_the_device> <filepath_of_your_computer_desktop>`

- 请与您的经销商或赫星官方联系，发送错误报告的.zip文件日志。错误报告必须随附有关发生的详细情况信息：哪个应用程序引起了问题，问题的描述，在什么情况下，您进行的一些什么设置和拍摄视频，照片等..以及所有可能有助于测试维修人员解决问题的相关信息，谢谢。



> 后续更新请关注CubePilot官方网站：
>
> https://docs.cubepilot.org/user-guides/herelink/herelink-overview

![20200320168](assets/20200320168.png)