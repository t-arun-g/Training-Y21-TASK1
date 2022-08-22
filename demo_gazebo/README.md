HOW TO RUN
==
1. First open the catkin workspace (here : sim_ws)
2. Then build the project using catkin_make
3. run $ source ./devel/setup.bash
4. launch the project using launch file : $ roslaunch demo_gazebo world.launch
5. add the plugins in the rviz
6. save the rviz file
7. add any models in gazebo environment to test if laser works properly
8. use map_server package to save the map.

    
    
HOW I MADE IT
==
1. make a package demo_gazebo and make folders : models,launch,world
2. used my old xacro and gazebo files from previous assignment.
3. added camera joint and then camera in xacro file {repeat for another camera}
4. added the imu joint and imu in the same way
5. I gave them shapes as cube
6. added the laser and set its visualize to true to see the blue laser and how its blocked
7. All the plugins were added in the gazebo file and the syntax were used from the website.
8. added the gmapping node in the launch file and set its scan property to my respective laser scan topic where it publishes data
9. used the command $rosrun map_server map_saver -f map to get the image of the gmap


LINK TO MY YOUTUBE VIDEO : https://youtu.be/MsiLmhWLNtA
