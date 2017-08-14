# slam_karto_g2o

A ROS Package for Pose Graph SLAM that uses open_karto for the front end and g2o for backend

# Acknowledgement

This package would not have been possible without the nav2d package by Sebastian Kasperski (https://github.com/skasperski/navigation_2d)

# Notes

The optimization routine used is Levenberg-Marquadt provided by g2o, you can easily change it to something else (Powell's dog leg etc.)

# How-To Use

Use the given launch files. The build_map_w_params launch files uses a given param file, which you can edit to change the behavior of open_karto. Make sure to use the right scan topic. Also, the package will expect odometry to be published to the /odom topic.

# Dependencies

* g2o: https://github.com/RainerKuemmerle/g2o
* SuiteSparse: www.suitesparse.com
* EIGEN

# Support

Head on over to my blog post http://sauravag.com/2017/07/an-practical-introduction-to-pose-graph-slam/ where you can ask questions and I will try to respond in a timely manner.
