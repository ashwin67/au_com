---
layout: post
title: Turtlebot goes round and round
date: 2018-04-18
type: post
parent_id: '0'
published: true
password: ''
status: publish
categories:
- New
- Robotics
author:
  login: ashwin67
  email: ashwin67@gmail.com
  display_name: ashwin67
  first_name: Ashwin
  last_name: Upadhyaya
---
Last post, we saw what was happening in the background when the turtlebot was moving around. Now, we try to modify the behaviour programatically. <!--more--> If you are using C++, the [Ros Wiki](http://wiki.ros.org/ROS/Tutorials) should be sufficient. If you are using python, the [Rospy tutorials](http://wiki.ros.org/rospy_tutorials/Tutorials) are also necessary. Create a new package in catkin_ws/src, write some code (I copied the turtlebot3_teleop and made suitable modifications), catkin_make and install and you should be ready to go. 

My code is available here: [https://github.com/ashwin67/roxperiments/tree/master/turtlebot3_round](https://github.com/ashwin67/roxperiments/tree/master/turtlebot3_round)

Once you have successfully completed make and install, you just need to run the various ROS commands in separate consoles:

|~$ roscore | 

|~$ export TURTLEBOT3_MODEL=burger |
|~$ roslaunch turtlebot3_bringup turtlebot3_remote.launch |

|~$ roslaunch turtlebot3_bringup turtlebot3_remote.launch |

|~$ rqt | 

|~$ ssh turtlebot3@192.168.x.xxx |
|~$ roslaunch turtlebot3_bringup turtlebot3_robot.launch |

And here is the robot running around in circles:
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/pG8rMMF1eG8" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
