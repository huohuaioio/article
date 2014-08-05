# 可控可监测温度的电饭锅

>[原文链接] (http://www.instructables.com/id/Cheap-and-effective-Sous-Vide-cooker-Arduino-power/?ALLSTEPS)  作者:Etienne Giust 翻译:AD（ldq370125）

标签（空格分隔）： 

---

![](http://huohua.qiniudn.com/SousVideCooker01.jpg)

![](http://huohua.qiniudn.com/SousVideCooker02.jpg)

##1 简介

是不是在做饭的时候，经常会出现糊锅的状况？
做饭的时候，必须要时刻的盯着饭锅？
做饭的时候，是不是会担心锅内的温度到底是高了？低了？还是正好呢？

这所有的问题，都不是事！
下面跟着我一起做一个可控可监测温度的电饭锅吧！

##2 清单
###2.1 材料
- Arduino UNO X1
- 8位LED显示模块（MAX7219） X1
- 压电蜂鸣器 X1
- 数字温度传感器DS18B20 X1
- 4.7kΩ电阻 X1
- 5V继电器（AC 125/250V） X1
- 电饭煲 X1

###2.2 工具
- 手钻 X1
- 电烙铁 X1
- 木板 X1
- 塑料保护壳 X1


##3 组装
###3.1 将温度传感器添加到盖子上
- 首先要在锅盖上打一个洞，最好是在中央位置，将温度传感器通过该洞放进去。

![](http://huohua.qiniudn.com/SousVideCooker04.jpg)

- 线长要保证传感器能够浸在水的中央。

![](http://huohua.qiniudn.com/SousVideCooker05.jpg)

- 如果有条件的话，可以将温度传感器包裹在一个“铁丝笼”里面，这样就可以保证饭锅在加热食物的时候，温度传感器可以与凉的食物隔离开，从而准确地测量水温。

![](http://huohua.qiniudn.com/SousVideCooker06.jpg)

###3.2 添加继电器
- 为了保证安全，我们最好是使用继电器来连接、断开高压电路。首先是要找到电饭锅的电源线，断开其中一根线，接入继电器。

![](http://huohua.qiniudn.com/SousVideCooker07.jpg)

![](http://huohua.qiniudn.com/SousVideCooker08.jpg)

- 我们需要找一块适当大小的木板，将继电器固定起来，如下图所示。

![](http://huohua.qiniudn.com/SousVideCooker09.jpg)


- 最终，我们需要使用一个透明的塑料可以开关的盒子，将继电器密封起来，这样就能够保证我们的用电安全了。

####注：这一步非常关键，能够确保我们的人身安全。

![](http://huohua.qiniudn.com/SousVideCooker10.jpg)



###3.3 连接电路
布线比较简单，按下面步骤来：

=====输入端=====

按钮1：

- 一端接地，另一端接pin 6

按钮2：

- 一端接地，另一端接pin 5

温度传感器：

- 红线接5V
- 黑线接地
- 另一根线（黄色或者白色）接pin 9

=====输出=====

压电蜂鸣器：

- 一端接地，另一端接pin 13

继电器：

- VCC接5V
- GND接地
- 控制线接pin 8

8位LED显示屏：

- VCC接5V
- GND接地
- DataIn接pin 12
- CLK接pin 11
- load接pin 10

连接后实物图：

![](http://huohua.qiniudn.com/SousVideCooker11.jpg)

###4 代码

代码下载地址[链接]


###5 加装支架

我们做这个温度控制电饭锅，主要是要利用锅里面的液体加热，而非电饭锅直接加热，所以我们可以找一个不锈钢框架，减掉大的部分，放置到锅的底部。如下图所示。

![](http://huohua.qiniudn.com/SousVideCooker12.jpg)

![](http://huohua.qiniudn.com/SousVideCooker13.jpg)

###6 享受美食吧

- 利用按钮2来设置目标温度（50℃到90℃之间）
- 实际的温度可以实时的显示在Led显示屏上
- 初始加热阶段建议不要打开锅盖
- 蜂鸣器响的时候，就可以打开锅盖，放入你的食物

好了，开始ENJOY IT！ENJOY YOUR FOOD！

![](http://huohua.qiniudn.com/SousVideCooker14.jpg)