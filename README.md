# UdacityProject3 "Map my World"

Course Project from Robotics Software Engineer - Mapping and SLAM. 
In this project I create 2D occupancy grid and 3D octomap from a simulated environment using my own robot with the RTAB-Map package.
## What does it do:
1. Develop package to interface with the rtabmap_ros package.
2. Add RGB-D camera.
3. Create the launch files to launch the robot and map its surrounding environment.
4. Move around the room to generate a proper map of the environment.
5. Perform localization using the created map.

To launch world:
<pre>
roslaunch my_robot world.launch
</pre>

To launch mapping:
<pre>
roslaunch my_robot mapping.launch
</pre>

To launch localization:
<pre>
roslaunch my_robot localization.launch
</pre>

To launch teleop:
<pre>
rosrun teleop_twist_keyboard teleop_twist_keyboard.py
</pre>
