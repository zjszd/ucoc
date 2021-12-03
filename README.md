# ucoc
1. 学习嵌入式实时操作系统（RTOS）,以uc/OS为例，将其移植到stm32F103上，构建至少3个任务（task）:其中两个task分别以1s和3s周期对LED等进行点亮-熄灭的控制；另外一个task以2s周期通过串口发送“hello uc/OS! 欢迎来到RTOS多任务环境！”。记录详细的移植过程。



参考：

1) https://blog.csdn.net/weixin_43116606/article/details/105532222

STM32F103C8T6移植uC/OS-III基于HAL库超完整详细过程

2) https://blog.csdn.net/junseven164/article/details/121534916

3) https://blog.csdn.net/qq_45659777/article/details/121570886   (踩坑较多，总结详细，推荐阅读)





2. 了解实时时钟RTC的原理。STM32芯片自带RTC，因此不须像其他MCU需外接RTC模块。请编程实现STM32的日历读取、设置和输出。要求：

1）读取RTC初始时间，验证是否为 1970年1月1日零分零秒；

2）将RTC时间调整为当前时间，并以 2021年x月x日x分x秒的格式从串口输出(或输出到OLED屏)，每1s改变一次；

3）如果输出内容中需加入“星期x”，请修改代码。



参考：

 https://www.cnblogs.com/dreamrj/p/14046598.html

[STM32系列]HAL库STM32CubeMX教程十三---RTC时钟

https://blog.csdn.net/as480133937/article/details/105741893



3. 在上述实验中，在掌握Keil的仿真调试代码功能之外，也学习使用仪器对代码运行进行故障排查和功能调测。

1) 练习使用示波器去观察LED输出电平和串口通信的波形，分析故障；

2) 分别使用Keil虚拟仿真逻辑仪和 真实逻辑仪(SaleaeLogic16)抓取LED输出电平和串口通信的波形，进行协议分析。 

附件：

SALEAELOGIC16_(逻辑分析仪软件与说明书-可安装最新版软件，但须先看旧版软件目录下中文指南中的串口分析案例).rar
