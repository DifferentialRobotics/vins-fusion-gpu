<img src="images/nus_logo.png" alt="nus logo" align="right" height="80" />

# vins-fusion-gpu

## 概述
本项目为**微分智飞**公司旗下教育无人机子品牌**非凸空间**适配的双目定位算法，其基于开源算法 **[VINS-Fusion-gpu](https://github.com/pjrambo/VINS-Fusion-gpu)** ，并集成了realsense相机的ros驱动**[realsense-ros](https://github.com/realsenseai/realsense-ros)**。相关readme见[readme-vins](vins-fusion-gpu/README.md)和[readme-realsense](vins-fusion-gpu/realsense-ros/README.md)。

## 项目拉取
```
cd ~/workspace/src
git clone https://github.com/DifferentialRobotics/vins-fusion-gpu.git

cd ~/workspace
catkin_make
```

## 程序运行
```
cd ~/workspace
source devel/setup.zsh  # 如果使用bash终端，则执行: source devel/setup.bash
roslaunch realsense2_camera rs_camera.launch #启动相机驱动
roslaunch vins vins_d435.launch #使用d435相机定位
```


## 致谢与声明
本项目使用了 **[VINS-Fusion-gpu](https://github.com/pjrambo/VINS-Fusion-gpu)** 和 **[realsense-ros](https://github.com/realsenseai/realsense-ros)**，特此感谢相关作者团队的开源贡献。

相关代码均严格遵循原项目的开源许可协议使用，用户在使用本项目时，请务必遵守相应的许可证条款。

# Q&A
请随时提交问题或讨论，我们会在看到问题后尽快回复。
