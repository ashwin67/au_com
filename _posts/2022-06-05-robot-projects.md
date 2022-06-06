---
layout: post
title: Robot projects
date: 2022-06-05
img: thumbnails/lawnmower.jpg
---

It was 2010 when I got a job at Bosch to work on a "cutting edge" lawnmower, now called the Bosch Indego. At that point, there was only one famous robotic lawnmower, the Husqvarna. They had very smartly patented a critical piece of technology, the perimeter wire which would be laid at the borders of a lawn which would sense and thereby help a lawnmower stay inside the lawn. Without this, it was quite hard to safely prevent a lawnmower from trying to mow the street or the neighbor's garden. Once the patent expired, there were a slew of lawnmowers about to enter the market and Bosch wanted to be at the forefront. The PhD experts had figured out the mathematics, algorithms, sensors etc required to realize such a thing and our job was to make this robot real.

![Bosch Lawnmower](/assets/robots/lawnmower.png "Bosch lawnmower")

The Husqvarna was a robot that simply went in random directions. It would move in a straight line, detect the perimeter wire and randomly turn in a different direction and continue to mow. The marketing take was that it acted like sheep which grazed randomly but ensure the grass would be perfect. Bosch wanted to make the perfect lawnmower, one which created those perfectly parallel lines in the lawn. With the usual accelerometer and gyroscope sensors, kalman and A star algorithms, we indeed made such a robot. It would learn the shape of the lawn during installation and plan its path, avoid obstacles and cleverly go around them. It could handle a tilted lawn and it would work in the rain. When it was released, I believe it was the best product in the market.

As for me, this got me hooked into the world of robots. Bosch wanted to make a digital kitchen assistant called Mykie. Think of it like Amazon alexa but with a face and a projector to beam videos on a wall. Based on a microphone array, it would detect the direction from which a user talked, turn its head towards them and reply. If they asked for something, it would project the information on a wall. However, it is hard today to compete with Silicon valley when it comes to these technologies. The outcome was only a few dozen prototypes but it was a lot of fun for us engineers.

![Mykie](/assets/robots/mykie.jpg "Digital assistant robot Mykie")

But most of the fun with building robots is at home. The turtlebot helped me learn ROS. The AR3 is a 6 DOF robot which can actually do some heavy lifting. My son uses his lego boost to learn some code.

![AR3 6 DOF Robot](/assets/robots/AR3.jpg) ![Lego Boost](/assets/robots/boost.jpg)

It is more than twelve years since I first started to play around with robots. The biggest difference I see between then and now is the ease with which an engineer can start a project. There is ROS for the software side of things. So many open source projects to choose from. 3D printers to help you build the structure. Aliexpress from where you can easily source any component. Deep learning frameworks and pre-trained models for speech and image recognition. None of these were available twelve years back. There was never a better time to actually build a robot.

![ROS](/assets/robots/ros.png) ![3d printer](/assets/robots/3dprinter.jpg)