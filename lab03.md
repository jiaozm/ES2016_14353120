# Lab3:DOL实例分析&编程
需要用到Make工具，Ant工具以及Java
***
## 实验理解：
1、在dol文件夹，有一个examples的文件夹，下面包含着各种运行的实例。这次的实验就是对于这些样例的修改。
2、在example1中定义了一个平方进程，对于代码：
![](https://raw.githubusercontent.com/jiaozm/ES2016_14353120/master/lab3_pic/1.png) <p>
p->local->index是指当前的位置，该值被初始化为0；p->local->len为生产者的长度，若满足当前位置小于生产者的长度，则对变量i进行平方运算。
本次实验修改这部分为i*i*i即可。
3、而example2，就是就是通过迭代的方式，循环三次来生成connection，从而得到i 8的运算结果。这次只用输出两个模块。那么只要将<variable value="3" name="N"/>中的3改为2即可。

## 实验过程
#### 1、修改example2，让3个square模块变成2个：
    只要将<variable value="3" name="N"/>中的3改为2即可。
修改文件：
![](https://raw.githubusercontent.com/jiaozm/ES2016_14353120/master/lab3_pic/2.png) <p>
结果：
![](https://raw.githubusercontent.com/jiaozm/ES2016_14353120/master/lab3_pic/3.png) <p>
得到的dot图为：
![](https://raw.githubusercontent.com/jiaozm/ES2016_14353120/master/lab3_pic/4.png) <p>
#### 2、修改example1，使其输出3次方数。
修改文件：
![](https://raw.githubusercontent.com/jiaozm/ES2016_14353120/master/lab3_pic/5.png) <p>
实验结果：
![](https://raw.githubusercontent.com/jiaozm/ES2016_14353120/master/lab3_pic/6.png) <p>

## 实验感想：
  这次实验只要根据ppt的提示，修改两行代码即可。但是也需要学习dol下example的实例具体的运行和框架，才能很好的完成实验。而且也回忆了markdown的一些使用方法。
	总之这次实验也让我获益匪浅。



