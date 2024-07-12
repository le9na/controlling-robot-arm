# ✨ Controlling Robot Arm in ROS Noetic ✨
## *Using MoveIt and Joint State Publisher Packages to Control a Robot Arm in Simulation* 🌟

### *Before Starting!*
*Sourcing ROS noetic:*

```
source /opt/ros/noetic/setup.bash
```

*We should start by setting up our workspace and installing needed packages using these commands in the terminal:*

```
mkdir -p ~/catkin_ws/src
cd ~/catkin_ws/
catkin_make

source devel/setup.bash

cd ~/catkin_ws/src
sudo apt install git
git clone https://github.com/smart-methods/arduino_robot_arm 

cd ~/catkin_ws
rosdep install --from-paths-src --ignore-src -r -y
sudo apt-get install ros-noetic-moveit
sudo apt-get install ros-noetic-joint-state-publisher ros-noetic-joint-state-publisher-gui
sudo apt-get install ros-noetic-gazebo-ros-control joint-state-publisher
sudo apt-get install ros-noetic-ros-controllers ros-noetic-ros-control

catkin_make
```

![Screenshot_1](https://github.com/user-attachments/assets/c8bfadf6-cce2-4fcc-a52f-03caae67702b)

![Screenshot_2](https://github.com/user-attachments/assets/6c955fc8-7bf7-4afb-87eb-3080069cb718)

![Screenshot_3](https://github.com/user-attachments/assets/615b6d82-3f0c-4768-9797-10f61a0174f4)

![Screenshot_4](https://github.com/user-attachments/assets/91a7ee43-4433-4401-939f-277fae991e49)

![Screenshot_5](https://github.com/user-attachments/assets/a7f4b542-9520-4706-9724-743363ff9764)

![Screenshot_6](https://github.com/user-attachments/assets/8a5ddfd0-9611-4731-80d5-3f9a89681177)

![Screenshot_7](https://github.com/user-attachments/assets/1343db40-fb85-44dc-b1a6-3f8db09198bd)

-------------------------------------------------------------------------------------------------

### 1. *Using Joint State Publisher:* ⚡

*Using the command:*

```
roslaunch robot_arm_pkg check_motors.launch
```

![Screenshot_8](https://github.com/user-attachments/assets/12fada71-e63b-428e-88a0-9aa6f5dda201)

-video-

-------------------------------------------------------------------------------------------------

### 2. *Using MoveIt Package (With gazebo simulation)*: ⚡

*Using the command:*

```
roslaunch moveit_pkg demo_gazebo.launch
```

![Screenshot_9](https://github.com/user-attachments/assets/cc8ff45c-9878-4583-8c1d-026a99863bb7)

-video-

Uploading gazebo.mp4…



*That's it!* 🐻
