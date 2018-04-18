---
layout: post
title: All the data between ROS and Turtlebot
date: 2018-04-14
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
Now that the turtlebot is running, it is time to explore some internals. First you need to get the setup right. ROS should be installed correctly, network configuration should be ok and burger should be able to run. In 4 different consoles, you need to run the following: <br><!--more-->

| ~$ roscore | ~$ export TURTLEBOT3_MODEL=burger <br>~$ roslaunch turtlebot3_bringup turtlebot3_remote.launch |
| ~$ rqt | ~$ ssh turtlebot3@192.168.x.xxx <br>~$ roslaunch turtlebot3_bringup turtlebot3_robot.launch |

By doing the above, we are running ROS in the turtlebot, ROS in the remote machine and have also opened up a rqt window to browse through nodes, topics and anything else that you need. Something like this: 
![RQT Screenshot - ROS and Turtlebot]({{"/assets/turtlebot_rqt.jpg"}})
The RQT (and the ROS infrastructure) is pretty amazing if you have ever worked with proprietary robots where you will need to write hundreds of lines of logging code to get data out of the system. The RQT also provides some Robot Steering capabilities using GUI sliders.

It would be interesting to go into the details of each type of data; the type, range, frequency etc of each of the sensors.

Now that we have played with the data enough, it is time to write some code to publish values to one of the topics so that the robot can be moved around.
