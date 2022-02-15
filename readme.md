# ros-robot using jetson nano 

## this is my setting for my ros project
- Follow my project at  y blog https://kakeko.wordpress.com
- binding usb port https://msadowski.github.io/linux-static-port/ (dont forget restart)
ros distro melodic

- src ros_rplidar https://github.com/robopeak/rplidar_ros
- source devel/setup.bash


## Command
- roscore
- roslaunch rplidar_ros rplidar.launch
- roslaunch rplidar_ros view_rplidar.launch
- roslaunch hector_slam_launch tutorial.launch
- rosrun rosserial_python serial_node.py /dev/ttyUSB1 (USB Arduino port)
- rosrun teleop_twist_keyboard teleop_twist_keyboard.py
]



# reference
- https://www.youtube.com/watch?v=HLLmV9LQoac&ab_channel=JamesBruton (howto use odom using arduino mega)
- https://github.com/RBinsonB/Nox_robot

# TIPS
- rosdep install --from-paths src --ignore-src -r -y
- rebuild when catkin_make have some problem cannot find file in src (delete build and devel and catkin_make)
- check /dev/tty info udevadm info /dev/ttyUSB1
