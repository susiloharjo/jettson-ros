# ros-robot using jetson nano 

## this is my setting for my ros project
- Follow my project at  y blog https://kakeko.wordpress.com
- binding usb port https://msadowski.github.io/linux-static-port/ (dont forget restart)
ros distro melodic

src ros_rplidar https://github.com/robopeak/rplidar_ros
source devel/setup.bash
roscore
roslaunch rplidar_ros rplidar.launch
roslaunch rplidar_ros view_rplidar.launch
roslaunch hector_slam_launch tutorial.launch


