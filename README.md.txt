blink是第一个作业，采用delay(250)实现闪烁
exti2是按钮进行控制的作业，采用EXTI_Callback,通过switch,case判断（b站学习）
NODELAY是没有采用delay进行灯泡闪烁，采用计时器的中断
change2是拓展作业一，采用主循环状态机轮询，判断按下，闪烁两种状态，用计时器中断实现闪烁效果
double 是拓展作业二
stm_homework2是第二次作业：
   change2是作业一，采用主循环状态机轮询，判断按下，闪烁两种状态，用计时器中断实现闪烁效果
   ledmotion是作业二：PSC=71 ARR=9999 
   按作业要求占空比是5%到25%，舵机对应脉宽为0.5ms ，2.5ms,可知应设置舵机周期为0.01s,频率为100hz，72000000/72/10000=100
   CRR从500增加到2500即可

   ADC是转换电压值，作业三

   breath_change 作业四，与作业一不同，全部采用中断写法

   controlmotion是作业五   由作业二可知0度时CRR=500对应adc,180度时CCRR=2500对应adc4095，
                                        可得函数CRR=0.488*adc+500






