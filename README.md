# Hugo Coding Challenge

For this challenge you need to have ROS2 installed(or docker). Provided with this file there is a ROS2 bag file, a database with data of Hugo’s sensor output during a test drive. The center of the robot is inbetween the two wheels. 

**(Easy)** For the first assignment you should read the wheel speeds from the bagfile, either make a ros subscriber that listens to the data or just run ‘ros2 topic echo’ and print the data to the terminal. And then you will use this data to plot the ``(x,y)`` positions of the robot. Plot the path and view it as an image, graph or your own personal favorite viz framework.


**(Medium)** Here we want you to extract the LaserScans as well and project them around the ``(x,y)`` position from the previous question. To project them out you need to know where the robot is (x,y) and the direction of the robot(current minus previous position should do fine).


**(Ultra hard)** Here we want you to fuse LaserScan data with wheel speeds using a kalman filter(of your choice), to improve the ``(x,y)`` estimations from the first question. Plot the new and improved path.

## Robot dimensions(metric)
* wheel_radius: 0.135
* track_width: 0.67

## Submit

Send your code and results(images/plots) to ggwp@hugo.tech.

### References

https://docs.ros.org/en/foxy/Tutorials/Ros2bag/Recording-And-Playing-Back-Data.html

