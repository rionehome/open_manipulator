# open_manipulator

## setup

```
$ sudo apt install python3-rospkg
$ sudo apt install ros-dashing-python* ros-dashing-rqt*

$ cd ~/ros2_ws/src
$ git clone -b ros2 https://github.com/ROBOTIS-GIT/DynamixelSDK.git
$ git clone -b ros2 https://github.com/ROBOTIS-GIT/dynamixel-workbench.git
$ git clone -b ros2 https://github.com/ROBOTIS-GIT/open_manipulator.git 
$ git clone -b ros2 https://github.com/ROBOTIS-GIT/open_manipulator_msgs.git
$ git clone -b ros2 https://github.com/ROBOTIS-GIT/open_manipulator_dependencies.git
$ git clone -b ros2 https://github.com/ROBOTIS-GIT/robotis_manipulator.git

$ cd ~/ros2_ws && colcon build --symlink-install
```

## run 

```
$ source ~/ros2_ws/install/local_setup.bash 
$ ros2 run open_manipulator_x_controller create_udev_rules 
$ ros2 launch open_manipulator_x_controller open_manipulator_x_controller.launch.py 

$ source ~/robotis_ws/install/local_setup.bash 
$ ros2 run open_manipulator_x_teleop open_manipulator_x_teleop_keyboard
```
