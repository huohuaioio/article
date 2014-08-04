# 逗猫神器

>[原文链接] (http://www.instructables.com/id/Remote-Control-Cat-Harness/?ALLSTEPS) 作者:Aleator777   翻译:AD（ldq370125）

标签（空格分隔）： 激光笔 逗猫

---

![](http://huohua.qiniudn.com/PlayWithCat01.jpg)

![](http://huohua.qiniudn.com/PlayWithCat02.jpg)

##1. 简介
还在用狗尾草逗猫玩么？
还在让你家的猫咪大人玩线球么？
是不是觉得传统逗猫玩的东东都已经弱爆了啊！
想不想来点刺激好玩的呢？
那就来看这儿的这个逗猫神器吧！
    
##2. 清单
###2.1 材料
- 遥控直升机 X1
- 激光笔 X1
- 伺服电机 X1
- NPN晶体管 X1
- 1kΩ电阻 X1
- AAA电池座 X1
- AAA电池 X2
- AA电池 X6
- 猫咪束缚带 X1
- 猫咪 X1
- 导线若干
- 针线

![](http://huohua.qiniudn.com/PlayWithCat03.jpg)

###2.2 工具
- 螺丝刀
- 尖嘴钳
- 电烙铁
- 3D打印机
- 台钳

##3. 组装
### 3.1 改装遥控直升机
我们改装遥控直升机，其实主要是要得到其内部的红外收发组件，用以控制我们的伺服电机转动以及激光的开关。

- 先来一张整个遥控直升机的完全拆解图

![](http://huohua.qiniudn.com/PlayWithCat04.jpg)

- 下面就是待我们任意宰割的遥控直升机“全尸”！

![](http://huohua.qiniudn.com/PlayWithCat05.jpg)

- 我们先从底部下手，拆解下来底座

![](http://huohua.qiniudn.com/PlayWithCat06.jpg)

- 已经拆下很多东东了，不要心疼自己的直升机哦

![](http://huohua.qiniudn.com/PlayWithCat07.jpg)

- OK！这儿就基本把主要的红外收发组件拆了出来

![](http://huohua.qiniudn.com/PlayWithCat08.jpg)

- 将螺旋桨等部件一一拆下

![](http://huohua.qiniudn.com/PlayWithCat09.jpg)

### 3.2 改装伺服电机
我们将使用红外收发组件直接控制伺服电机的转动，所以我们这儿就是需要将原装伺服电机里面的控制板拆出来。

- 先来一张原装的伺服电机照片

![](http://huohua.qiniudn.com/PlayWithCat11.jpg)

- 在伺服电机的下方可以看到四个小螺丝起固定作用

![](http://huohua.qiniudn.com/PlayWithCat12.jpg)

- 用螺丝刀将4个小螺丝拆解下来，打开伺服电机的后盖

![](http://huohua.qiniudn.com/PlayWithCat13.jpg)

- 伺服电机里面的控制主板一眼就可以看到，小心的拉出来

![](http://huohua.qiniudn.com/PlayWithCat14.jpg)


- 将控制主板拆解掉，只剩下下图中部件的样子

![](http://huohua.qiniudn.com/PlayWithCat15.jpg)

- 找一对10cm左右的导线

![](http://huohua.qiniudn.com/PlayWithCat16.jpg)

- 将这两根导线跟剩下的伺服舵机的两根线头焊接在一起

![](http://huohua.qiniudn.com/PlayWithCat17.jpg)

- 盖上后盖，将4个螺丝拧上

![](http://huohua.qiniudn.com/PlayWithCat18.jpg)

- 3D打印出伺服舵机的底座（3D打印源文件 [链接](http://huohua.qiniudn.com/PlayWithCat01.stl)）

![](http://huohua.qiniudn.com/PlayWithCat19.jpg)

- 将改装后的伺服电机安装在底坐里面，并将引线伸出来

![](http://huohua.qiniudn.com/PlayWithCat20.jpg)

### 3.3 改装激光笔

我们需要将激光笔改成体积稍小的组件，所以拆解激光笔必不可少。

- 这儿我们需要一根激光笔和相应的工具

![](http://huohua.qiniudn.com/PlayWithCat21.jpg)

- 用台钳把激光笔固定住

![](http://huohua.qiniudn.com/PlayWithCat22.jpg)

- 将激光笔的激光头给钳下来

![](http://huohua.qiniudn.com/PlayWithCat23.jpg)

- 这个过程还是稍微有点暴力的，要用到台钳和钳子。注意安全。

![](http://huohua.qiniudn.com/PlayWithCat24.jpg)

- OK！拆解出来了。

![](http://huohua.qiniudn.com/PlayWithCat25.jpg)

- 这就是我们最需要的激光头部分。怎么样，这样就小巧多了吧！

![](http://huohua.qiniudn.com/PlayWithCat26.jpg)

- 我们需要将两条控制线焊接在激光头上

![](http://huohua.qiniudn.com/PlayWithCat27.jpg)

- 更清楚点的焊接照片

![](http://huohua.qiniudn.com/PlayWithCat28.jpg)


### 3.4 合体

- 首先是我们整体的电路原理图，或者叫做框架图也行。

![](http://huohua.qiniudn.com/PlayWithCat29.jpg)

- 下一步就是要按照这个清晰的原理图把各个组件连接起来，将激光头固定在伺服电机上，并且将电池座、红外遥控组件底座、伺服电机底座用针线缝在猫咪束缚带的背部一侧。（电池座源文件 [链接](http://huohua.qiniudn.com/PlayWithCat02.stl) 、红外遥控组件底座的源文件 [链接](http://huohua.qiniudn.com/PlayWithCat03.stl) )

![](http://huohua.qiniudn.com/PlayWithCat30.jpg)

- 组装起来后的另一侧照片

![](http://huohua.qiniudn.com/PlayWithCat31.jpg)

### 3.5 找一只猫咪

恩，这个说简单也简单，说难也难。。。

可爱的喵咪，赶紧到碗里来！

![](http://huohua.qiniudn.com/PlayWithCat32.jpg)


##4 成果展示

好啦！
给你家的猫咪安装这么一个高大上的玩具吧！
相信你家猫咪一定会爱死你的！

![](http://huohua.qiniudn.com/PlayWithCat33.jpg)

![](http://huohua.qiniudn.com/PlayWithCat34.jpg)












