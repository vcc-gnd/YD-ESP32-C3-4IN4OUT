# YD-ESP32-C3-4IN4OUT 控制器说明

###### 简介：

YD-ESP32-C3-4IN4OUT设备由源地工作室（VCC-GND Studio）设计，有需要可以浏览www.vcc-gnd.com获取购买。该设备使用ESP32-C3芯片，可以用于物联网应用的测试原型机也就可以用于实际应用，有4个按键输入和4个继电器输出构成。电源可以由100~240VAC或者9~24VDC供电，可以由433M手柄代替板子上的4个输入按键的功能，两个usb一个是硬件的usb转串口，一个是ESP32-C3的usb口。

![](/img/img2.PNG)

![](/img/img1.PNG)

###### 使用说明：

![](/img/img8.png)

###### 输入输出：

输入引脚说明

| 输入 | ESP32-C3对应引脚 | 说明                                  |
| ---- | ---------------- | ------------------------------------- |
| IN1  | GPIO0            | 轻触按键、433M控制输入                |
| IN2  | GPIO1            | 轻触按键、433M控制输入                |
| IN3  | GPIO8            | 轻触按键、433M控制输入                |
| IN4  | GPIO9            | 轻触按键、433M控制输入，ESP32-C3 BOOT |

输出引脚说明

| 输出 | ESP32-C3对应引脚 | 说明   |
| ---- | ---------------- | ------ |
| OUT1 | GPIO4            | 继电器 |
| OUT2 | GPIO5            | 继电器 |
| OUT3 | GPIO6            | 继电器 |
| OUT4 | GPIO7            | 继电器 |

###### USB口说明：

![](/img/img3.png)

USB1:方口USB，类型B母口，该口为USB转UART用途，连接ESP32-C3的TXD、RXD。使用芯片为CH340芯片，该可以用于ESP32-C3的调试和下载功能。例如下载更新TASMOTA固件。

![](/img/img9.png)

CH340芯片的驱动官方链接：

http://www.wch-ic.com/products/CH340.html?        ENGLISH

https://www.wch.cn/products/CH340.html?from=list     中文

USB2:该口为USB-A型母口，该USB为ESP32-C3的USB功能接口占用ESP32-C3的GPIO18\GPIO19，在pcb板上可以通过焊盘断开这个这两个USB通信线缆。该USB接口可以对外提供5V电源，所以可以插入WIFI热点。

![](/img/img4.png)

这2个USB都可以下载ESP32-C3固件程序。

![](/img/img5.png)

###### 电源说明：

该设备可以使用100~240Vac交流电源输入也可以使用9~24VDC直流电源。

![img7](/img/img7.png)

###### 下载软件：

如果下载TASMOTA固件，TASMOTA官方有自己的web下载。

https://tasmota.github.io/docs/

如果你下载自己的固件文件可以使用乐鑫的下载工具。

https://www.espressif.com.cn/en/home

