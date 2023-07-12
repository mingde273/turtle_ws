# 乌龟跟随

## 功能：

程序启动之初时产生两只乌龟，中间的乌龟(A) 和 左下乌龟(B), B 会自动运行至A的位置，并且键盘控制时，只是控制 A 的运动，但是 B 可以跟随 A 运行。

****

## 实现步骤：

1.  启动乌龟显示节点

2.  在乌龟显示窗体中生成一只新的乌龟(需要使用服务)

3.  编写两只乌龟发布坐标信息的节点

4.  编写订阅节点订阅坐标信息并生成新的相对关系生成速度信息

****
## 使用方法：
clone本项目到本地后开启两个命令行窗口，分别输入以下指令：

若使用C++ 文件：

```
roscore
```

```
cd 工作空间名(默认情况下为turtle_ws/)
catkin_make
source ./devel/setup.bash
roslaunch 功能包名(默认情况为turtle2turtle) test.launch
```

若使用python脚本：
```
roscore
```

```
cd 工作空间名(默认情况下为turtle_ws/)
source ./devel/setup.bash
catkin_make
roslaunch 功能包名(默认情况为turtle2turtle) test_p.launch
```
