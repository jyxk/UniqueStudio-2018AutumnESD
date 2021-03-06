zlc同学因为被810的门把手电晕,没有办法完成以下的题目,他把嵌入式的题交给了你:

# 背景简介:
## ESP8266

**ESP8266**是乐鑫公司开发的一款WiFi模组,但是坤谈里面的dalao很快发现,只拿这块玩意当wifi模组用太浪费了,于是在群众的要求下,官方放出了SDK包用于开发，而且使用官方的SDK可以让ESP8266不需要MCU便可单独运行.

## FreeRTOS

FreeRTOS是一个热门的嵌入式设备用实时操作系统核心,采用MIT许可证许可.它的设计小巧而简易,整个核心只有3到4个C文件,为了让代码容易阅读 移植和维护,大部分代码都是以C语言编写.提供了许多方法来实现多线程,多任务,互斥锁,信号量和软件计时器等等功能.

### ESP8266 RTOS SDK

该SDK是乐鑫公司开发的基于**FreeRTOS**的开发软件套件,在外设调用上与**ESP-IDF**官方库文件保持统一,同时支持**lwip**等低功耗的网络协议栈,并且支持阿里A-Link等通讯协议.

# 题目:
## 第一题: 
zlc同学不知道通过什么途(p)径(y)拿到了一块8266开发板,并且机缘巧合的发现这玩意有个SDK,于是zlc同学打算测试一下这块~~交易~~得到的板子是不是好的,准备编译一个官方的测试代码看看.

1. 自行安装ESP8266 RTOS SDK的开发环境,包括:**SDK源码包**和**编译调试工具链**
2. 编译并烧录位于SDK源码目录下`example/get_started` 目录下的实例代码
3. 使用编译,调试工具链自带的monitor和自行寻找的串口调试工具检查开发板的返回数据
4. 要求修改实例代码,使得开发板**每隔一定时间**返回`“Hello World”`字符串

### 提交内容 

+ 编译完的固件
+ 开发板返回字符串的截图
+ 自行修改的代码的源文件 

## 第二题 
zlc同学发现有人在偷听他和wls的机密谈话,感到很恼火,并且机缘巧合的发现手上有一个ESP8266开发板,于是准备发动自己的小脑筋,来解决有人偷听谈话的问题.

在第一题完成的基础上,利用RTOS实现以下功能两功能同时执行：
+ 让LED灯每隔**500ms**闪烁一次
+ 实现流式**摩尔斯电码转译**:利用开发板上的按钮（或外接按钮）输入摩尔斯电码,从串口输出字符串.

### 提交内容

+ 代码源码
+ 编译完的固件文件

# Hints:
+ www.google.com
+ www.github.com
+ www.freertos.org
+ https://www.espressif.com/zh-hans/products/hardware/esp8266ex/overview

你可能需要的文件:
+ https://drive.google.com/open?id=1cq5FKA8VXWzslgo1OAnx5bg1th57P2hL

# 评分标准:

**看心情**
