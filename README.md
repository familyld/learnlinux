#Linux 常用命令归纳

1. 显示日期的指令： date

```
lincoln@ubuntu:~/Learning/learnlinux$ date
2016年 04月 12日 星期二 10:39:52 HKT
```

2. 显示日历的命令：cal

```
lincoln@ubuntu:~/Learning/learnlinux$ cal
      四月 2016         
日 一 二 三 四 五 六  
                1  2  
 3  4  5  6  7  8  9  
10 11 12 13 14 15 16  
17 18 19 20 21 22 23  
24 25 26 27 28 29 30  
```

我们还可以在cal命令后带上一些参数以输出制定年月的日历，比如`cal 2016`可以输出2016年全年的日历，`cal 4 2016`可以输出2016年4月份的日历。

3. 简单的计算器：bc

```
lincoln@ubuntu:~/Learning/learnlinux$ bc
bc 1.06.95
Copyright 1991-1994, 1997, 1998, 2000, 2004, 2006 Free Software Foundation, Inc.
This is free software with ABSOLUTELY NO WARRANTY.
For details type `warranty'. 
1+2+3+4
10
10%3
1
10/100
0
scale = 3
10/100
.100
quit
```

bc计算器可以进行加减乘除以及求模等运算，默认输出到整数位，如果需要输出小数，就要设置`scale=number`，number就是我们希望输出的小数位的位数。(然而感觉直接进入python更实用..)

4. 重要的几个热键[Tab], [ctrl]-c, [ctrl]-d 

[Tab]按键---具有补全的功能，如果连按两次会列出所有以输入开始的命令，比方说：

```
lincoln@ubuntu:~/Learning/learnlinux$ cal [连按两下Tab]
cal            calendar       calibrate_ppa  caller 
```

[Ctrl]-c按键---让当前的程序『中止』。

[Ctrl]-d按键---通常代表着：『键盘输入结束(End Of File, EOF 戒 End OfInput)』的意思；另外，也**可以用来取代输入exit或者quit**。

5. 查看使用手册的命令 man

```
lincoln@ubuntu:~/Learning/learnlinux$ man cal
```

在回车以后，命令行界面会跳转到手册页面，也即介绍命令怎么用的界面，比方说上面的`man cal`，回车以后，就会跳到介绍cal的使用方法的界面，手册是linux自带的。我们还可以通过下面这样的方式来使用：

```
lincoln@ubuntu:~/Learning/learnlinux$ man -f man
man (1)              - 在线参考手册的接口
man (7)              - macros to format man pages
```

加入`-f`参数后会显示关键字的一些描述信息，这里显示man命令的手册第1章和第7章分别描述了什么功能，我们可以根据描述选择我们要看手册的第几章，然后通过`lincoln@ubuntu:~/Learning/learnlinux$ man 章节号  man`的方式来直接查看手册的某一章。



