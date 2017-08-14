# slam_karto_g2o
A ROS Package for Pose Graph SLAM that uses open_karto for the front end and G2O for backend

This package would not have been possible without the nav2d package by Sebastian Kasperski (https://github.com/skasperski/navigation_2d)

The optimization routine used is Levenberg-Marquadt, you can easily change it to something else (Powell's dog leg etc.)
