# ROS_MATLAB_ROStoolbox
# Dscription
# Controlling a ROS-Enabled Robot using Matlab simulink:

-Reference: Examples by ROS Toolbox User’s guide(MATLAB 2017).

1.Creating own Two wheeled Differential Robot model.

  $ roslaunch ros_robotics diff_wheeled_gazebo_full.launch

2.Run simulink model

  $ sudo ./matlab

    Open the simulink model:
    >> open_system('Two_Wheeled_Robot_With_Default_Head_5.slx');

3.Configure Simulink to connect to the ROS network:

   Main menu-Tools-Robotic Operating System-Configure Ros Network address
   ROS Master section:
   -Hostname/IP add: 10.250.12.226 (ROS-Master)
   -Port: 11311

* TROUBLESHOOTING:

  -Execute following commands
   $ catkin_make
   $ source devel/setup.bash

 -Check for topic name by executing following command.
   $ rostopic list
     -Use the same topic names in a simulink model.
