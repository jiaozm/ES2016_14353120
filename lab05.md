# Lab5:����ROS
Ubuntu������
***

## ʵ�����
#### 1��
```
���source.list��
sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
���keys��
sudo apt-key adv --keyserver hkp://pool.sks-keyservers.net --recv-key 0xB01FA116
```
![](https://raw.githubusercontent.com/jiaozm/ES2016_14353120/master/lab5_pic/1.png) <p>
�����ͼ��
#### 2����װ��
����ȷ���������Debian��������������µģ�
sudo apt-get update  
���������氲װ�� ����ROS��rqt��rviz��ͨ�û����˺����⡢2D/3D�������������Լ�2D/3D��֪����
 sudo apt-get install ros-jade-desktop-full  
��ʼ��rosdep:
 sudo rosdep init
 rosdep update  
�������ã����ÿ�δ�һ���µ��ն�ʱROS�����������ܹ��Զ����úã�����ӵ�bash�Ự�У����ǽ��᷽��ܶ�
 echo "source /opt/ros/jade/setup.bash" >> ~/.bashrc
 source ~/.bashrc  
����㰲װ�ж��ROS�汾, ~/.bashrc ����ֻ�� source �㵱 ǰʹ�ð汾����Ӧ�� setup.bash�� 
�����ֻ��ı䵱ǰ�ն��µĻ�������������ִ����������
  source /opt/ros/jade/setup.bash  
��װrosinatall:rosinstall ��ROS��һ�������ֿ��ĳ��������й��ߣ������Է�������ͨ��һ������Ϳ��Ը�ĳ��ROS��������غܶ�Դ������ 
Ҫ��ubuntu�ϰ�װ������ߣ������У�
  sudo apt-get install python-rosinstall  
�����
![](https://raw.githubusercontent.com/jiaozm/ES2016_14353120/master/lab5_pic/2.png) <p>
#### 3������ROS��
��һ���նˣ�����ָ��roscore��
![](https://raw.githubusercontent.com/jiaozm/ES2016_14353120/master/lab5_pic/3.png) <p>
�򿪵ڶ����նˣ���������ָ�����һ��С�ڹ���棺rosrun turtlesim turtlesim_node
![](https://raw.githubusercontent.com/jiaozm/ES2016_14353120/master/lab5_pic/4.png) <p>
�ٴ�һ���նˣ�����rosrun rqt_graph rqt_graph�����Կ���ROS nodes�Լ�Topic��ͼ��չʾ��
![](https://raw.githubusercontent.com/jiaozm/ES2016_14353120/master/lab5_pic/5.png) <p>
#### 4��Cartographer���ã�
![](https://raw.githubusercontent.com/jiaozm/ES2016_14353120/master/lab5_pic/6.png) <p>
![](https://raw.githubusercontent.com/jiaozm/ES2016_14353120/master/lab5_pic/7.png) <p>
![](https://raw.githubusercontent.com/jiaozm/ES2016_14353120/master/lab5_pic/8.png) <p>
�Ҹ��ݽ̳�������������ʵ���ͼ��
![](https://raw.githubusercontent.com/jiaozm/ES2016_14353120/master/lab5_pic/9.png) <p>
![](https://raw.githubusercontent.com/jiaozm/ES2016_14353120/master/lab5_pic/10.png) <p>
���ܿ�ϧ��һ�����ÿ�ס�ˣ����Խ�����ȥ������Ҫ�Ͽε�ʱ������TA��

## ʵ����룺
  ����ʵ�������ɣ����д�Ŭ�������������ù�����Ҳ������ᵽ��cat������֮�������Ҷ���ʵ���ѧϰ�������˸���ֱ�۵��˽⡣



