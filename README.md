# installing-arm-package

## 1- create a folder named catkin_ws

$ mkdir ~p ~/catkin_ws/src  
$ cd ~/catkin_ws/  
$ catkin_make  

## 2- install the arm package by cloning smart-methods's repository

$ cd ~/catkin_ws/src  
$ git clone https://github.com/smart-methods/arduino_robot_arm.git  
$ cd ~/catkin_ws  

## 3- install dependencies

$ rosdep install --from-paths src --ignore-src -r -y  
$ sudo apt-get install ros-noetic-moveit  
$ sudo apt-get install ros-noetic-joint-state-publisher ros-noetic-joint-state-publisher-gui  
$ sudo apt-get install ros-noetic-gazebo-ros-control joint-state-publisher  
$ sudo apt-get install ros-noetic-ros-controllers ros-noetic-ros-control  

## 4- install Arduino from this link and unzip the folder

 https://www.arduino.cc/en/software  
 $ sudo ./install.sh
 
 ## 5- launch the robot arm by joint_state_publisher
 
 $ roslaunch robot_arm_pkg check_motors.launch  
 
 <img width="1080" alt="Screenshot 2022-08-23 234452" src="https://user-images.githubusercontent.com/86732926/186267271-7fda069d-b9f6-44b5-8803-ee3933eb5668.png">
 
