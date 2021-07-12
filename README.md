# using SLAM map to launch the navigation

* in navigation simulation you can choose a different enviroment and robot model in a navigation world ( like a SLAM simulation).

* this link will help you to do this [navigathion simulation in turtlebot3](https://emanual.robotis.com/docs/en/platform/turtlebot3/nav_simulation/)

* you must first finish from this [ turtlebot3 with SLAM simulation](https://github.com/raghad1912/task-2-Turtlebot3-with-SLAM-approach) to keep map saved because you must map  prepared before running the Navigation.


### so , the steps to do this task is : 
   * step 1 : launch a simulation world 
   * step 2 : run a navigation simulation 
   * step 3 : dealing with 2 D navigation goal 



### step 1 : launch a simulation world : 

<p><code> $ export TURTLEBOT3_MODEL=burger</code></p>
<p><code> $ roslaunch turtlebot3_gazebo turtlebot3_world.launch</code></p>


![task4opengazebo](https://user-images.githubusercontent.com/56357074/125214733-3b83f000-e2c1-11eb-99b2-8afee75033ba.png)




### step 2 : run a navigation simulation : 

<p><code> $ export TURTLEBOT3_MODEL=burger</code></p>
<p><code> $ roslaunch turtlebot3_navigation turtlebot3_navigation.launch map_file:=$HOME/map.yaml</code></p>

![task4openturtlebot3navigation](https://user-images.githubusercontent.com/56357074/125214730-39219600-e2c1-11eb-9fde-d3e8cb067ecb.png)



### step 3 : dealing with  2D navigation goal


  * go to ```2D nav goal ``` which is in the Rviz menu
  * then click on the map to set a destination that you want from robot go to it 

https://user-images.githubusercontent.com/56357074/125214712-29a24d00-e2c1-11eb-90a3-a2b64c87fd10.mp4

  * if you want , Launch keyboard teleoperation node to precisely locate the robot on the map.
<p><code> $ roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch</code></p>








https://user-images.githubusercontent.com/56357074/125214721-32931e80-e2c1-11eb-86a7-0169a4d58cc7.mp4


