# slam_karto_g2o

A ROS Package for Pose Graph SLAM that uses open_karto for the front end and g2o for backend.

# Acknowledgement

This package would not have been possible without the nav2d package by Sebastian Kasperski (https://github.com/skasperski/navigation_2d)

# Notes

The optimization routine used is Levenberg-Marquadt provided by g2o, you can easily change it to something else (Powell's dog leg etc.). This package is currently tested with Ubuntu 16.04 LTS + ROS Kinetic

# How-To Use

Use the given launch files. The build_map_w_params launch files uses a given param file, which you can edit to change the behavior of open_karto. Make sure to use the right scan topic. Also, the package will expect an odometry tf to be published to between odom frame and base_link (or base_footprint).

# Dependencies

* SuiteSparse: In ubuntu you can install as $ sudo apt-get install libsuitesparse-dev (www.suitesparse.com)

* Eigen: $ sudo apt-get install libeigen3-dev (most likely it is already installed if you have ROS)

* g2o: Downloand and install from https://github.com/RainerKuemmerle/g2o.

* Clone open_karto to your catkin_ws/src folder (https://github.com/ros-perception/open_karto)

# Support

Head on over to my blog post http://sauravag.com/2017/07/an-practical-introduction-to-pose-graph-slam/ where you can ask questions and I will try to respond in a timely manner.
