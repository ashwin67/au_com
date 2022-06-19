---
layout: post
title: A 3D printed 6 DOF robot
date: 2022-06-19
img: thumbnails/ar3.jpg
---

I decided to build a 6 DOF robot in January. Since mechanical engineering is not my cup of tea, I decided to use an open source project. After some research, I found [Chris Annin's AR3 robot](https://www.anninrobotics.com/home). You get all the 3D files, the component list of things to buy and also some basic software to run the robot. I had built robots at work but there was a whole team to do those. The hardware team would take care of schematics, component lists etc. The mechanical team would make the designs. The 3D printing of prototypes was outsourced. I was a system architect who knew the whole thing but lacked the details of everything.

The [AR3 robot manual](https://www.anninrobotics.com/downloads) described every step of the process with photos. I made a rough estimate of the costs and it added up to €2000. I found out how much the world depends on China when I could not buy certain parts anywhere else but in [aliexpress](aliexpress.com). Most items were available in amazon, digikey or reichelt but there is no way avoiding China for some critical parts such as pneumatic tubes for the robot's gripper. I found out that Europe also lacks the kind of choice available in the US when it comes to building things. A website like [mcmaster](https://www.mcmaster.com/) is just not available here. Naturally, I overshot my budget by about 15% as I had to pay a lot of customs and shipping. However, this budget also included the [anycubic 3D printer](https://www.anycubic.com/products/anycubic-vyper).

I 3D printed the parts with PLA and started building the robot as per the manual. There were several issues that had to be dealt with. For example,

- A lower setting of infill for 3D printing does not work for structural parts.
- Since the original design was for aluminium parts, some screws that worked for aluminium would not be long enough for PLA. I even broke a part after building the whole thing.
- Fitting a metal bearing ring into a PLA bearing ring holder is not the easiest of tasks. Normally, I use a hot air blower to soften the plastic just so much that it allows the metal ring to slide in. I lost at least one plastic piece because I heated it too much that it deformed completely.
- Set screws can give a lot of trouble if they lose their thread.
- and so on.

There were a lot of mistakes made but it is those mistakes that help you learn the most about building a robot. Finally, I have the robot. It calibrates when in open loop but has some issues with the encoder. The gripper still needs to be attached. I have to make it work with ROS. Probably there are some more mistakes to fix and some more things to learn.

![](/assets/robots/ar3_1.jpg) ![](/assets/robots/ar3_2.jpg) 
![](/assets/robots/ar3_3.jpg) ![](/assets/robots/ar3_4.jpg)