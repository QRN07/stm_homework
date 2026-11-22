blink是第一个作业，采用delay(250)实现闪烁
exti2是按钮进行控制的作业，采用EXTI_Callback,通过switch,case判断（b站学习）
NODELAY是没有采用delay进行灯泡闪烁，采用计时器的中断
change2是拓展作业一，采用主循环状态机轮询，判断按下，闪烁两种状态，用计时器中断实现闪烁效果
double 是拓展作业二
