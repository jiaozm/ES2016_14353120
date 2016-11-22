# Lab5:配置ROS
Ubuntu上配置
***

## 实验过程
#### 1、
```
添加source.list：
sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
添加keys：
sudo apt-key adv --keyserver hkp://pool.sks-keyservers.net --recv-key 0xB01FA116
```
![](https://raw.githubusercontent.com/jiaozm/ES2016_14353120/master/lab5_pic/1.png) <p>
结果如图。
#### 2、安装：
首先确保虚拟机的Debian软件包索引是最新的：
sudo apt-get update  
桌面完整版安装： 包含ROS、rqt、rviz、通用机器人函数库、2D/3D仿真器、导航以及2D/3D感知功能
 sudo apt-get install ros-jade-desktop-full  
初始化rosdep:
 sudo rosdep init
 rosdep update  
环境配置：如果每次打开一个新的终端时ROS环境变量都能够自动配置好（即添加到bash会话中），那将会方便很多
 echo "source /opt/ros/jade/setup.bash" >> ~/.bashrc
 source ~/.bashrc  
如果你安装有多个ROS版本, ~/.bashrc 必须只能 source 你当 前使用版本所对应的 setup.bash。 
如果你只想改变当前终端下的环境变量，可以执行以下命令
  source /opt/ros/jade/setup.bash  
安装rosinatall:rosinstall 是ROS中一个独立分开的常用命令行工具，它可以方便让你通过一条命令就可以给某个ROS软件包下载很多源码树。 
要在ubuntu上安装这个工具，请运行：
  sudo apt-get install python-rosinstall  
结果：
![](https://raw.githubusercontent.com/jiaozm/ES2016_14353120/master/lab5_pic/2.png) <p>
#### 3、测试ROS：
打开一个终端，输入指令roscore：
![](https://raw.githubusercontent.com/jiaozm/ES2016_14353120/master/lab5_pic/3.png) <p>
打开第二个终端，输入以下指令，开启一个小乌龟界面：rosrun turtlesim turtlesim_node
![](https://raw.githubusercontent.com/jiaozm/ES2016_14353120/master/lab5_pic/4.png) <p>
再打开一个终端，输入rosrun rqt_graph rqt_graph，可以看到ROS nodes以及Topic等图形展示：
![](https://raw.githubusercontent.com/jiaozm/ES2016_14353120/master/lab5_pic/5.png) <p>
#### 4、Cartographer配置：
![](https://raw.githubusercontent.com/jiaozm/ES2016_14353120/master/lab5_pic/6.png) <p>
![](https://raw.githubusercontent.com/jiaozm/ES2016_14353120/master/lab5_pic/7.png) <p>
![](https://raw.githubusercontent.com/jiaozm/ES2016_14353120/master/lab5_pic/8.png) <p>
我根据教程往下做，这是实验截图：
![](https://raw.githubusercontent.com/jiaozm/ES2016_14353120/master/lab5_pic/9.png) <p>
![](https://raw.githubusercontent.com/jiaozm/ES2016_14353120/master/lab5_pic/10.png) <p>
但很可惜有一步配置卡住了，难以进行下去，还需要上课的时候问问TA。

## 实验感想：
  本次实验较难完成，还有待努力！！但是配置过程中也让我体会到了cat的有用之处，让我对于实验课学习内容有了更加直观的了解。



