# Humanoid robot writes words

Team member: Di Zhu, Yixing Chen, Cheng Zhang
Date: May 3rd, 2016

The main goal of our project is to enable PR2 robot to write words using pen just like what human does in real life. The simulation is under ROS system with arm motion planning using MoveIt!.

### Project Structure
The project consists of three packages:
* robot_write - Move base towards the table + Grasp pen
* write_letter - Robot writes English alphabets based on user input
* points_and_lines - Display for letter in rviz

### Instruction

** Launch the project **:
```sh
$ cd PR2-handwriting
$ source /opt/ros/indigo/setup.bash
$ catkin_make
$ source devel/setup.bash
```

** robot_write **
```sh
$ rosrun robot_write robot_write
```

** write_letter **
```sh
$ rosrun robot_write robot_write
```

** points_and_lines (Display) **
```sh
$ rosrun rviz rviz &
Add 'Marker' layer in rviz
$ rosrun points_and_lines points_and_lines
```
Notes: 
Before using the program, please modify the path of txt file in write_letter.cpp and points_and_lines.cpp