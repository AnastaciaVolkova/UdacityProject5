# UdacityProject3 "Where Am I"

Course Project from Robotics Software Engineer - Localization. 
Demonstrates robot localization inside created before world with adaptive Monte Carlo algorithm (amcl).
## What does it do:
1. Launches the custom wolrd with robot.
2. Launches amcl node to localize the robot.
3. Launches move_base node to demonstrate robot localization

With help of <b>2D Nav Goal</b> botton in rviz gui user can set a goal and robot attempts to reach it.

In addition there is a possibility to control robot movements via teleop package.

To launch world:
<pre>
roslaunch my_robot world.launch
</pre>

To launch amcl and move base node:
<pre>
roslaunch my_robot amcl.launch
</pre>

To launch teleop:
<pre>
rosrun teleop_twist_keyboard teleop_twist_keyboard.py
</pre>
