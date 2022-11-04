# Gazebo_yolo_deepsort

## Installation
In order to install darknet_ros, clone the latest version into your catkin workspace and compile the package using ROS.

    cd ~/catkin_ws/src/
    git clone --recursive https://github.com/leggedrobotics/darknet_ros.git
    cd ../
    catkin build darknet_ros / catkin_make
    
    
In order to get turtlebot3:
  
    cd ~/catkin_ws/src/
    git clone https://github.com/ROBOTIS-GIT/turtlebot3_msgs.git
    git clone https://github.com/ROBOTIS-GIT/turtlebot3.git
    cd ~/catkin_ws && catkin_make
    
    
 ## To run
 You can always select which world you want to run under in /catkin_ws/src/turtlebot3_simulations/turtlebot3_gazebo/launch
 some addtional worlds are shown in the world package.
 
 Example of how to run:
 
 ### on first terminal
 
    source devel/setup.bash
    export TURTLEBOT3_MODEL=waffle
    roslaunch turtlebot3_gazebo turtlebot3_world.launch
    
 ### on second terminal
 
    source devel/setup.bash
    export TURTLEBOT3_MODEL=waffle
    roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch
    
 ### on third terminal
 
    source devel/setup.bash
    roslaunch darknet_ros yolo_v3.launch
    
 ## for Sort DeepSort, refer to:
 
 https://github.com/ilyasmg/sort-deepsort-yolov3-ROS#readme
 You can also clone from here, which resolve the indense issue of original repo

 
