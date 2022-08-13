# Arduino_Robot_Arm_V2_installation_guide


  this guide assumes that you have already installed the (Arduino Robot Arm)
   


## Installation steps: 

1- Download 3D modeling files from this link: https://drive.google.com/drive/folders/18E0vgwkuOhObBcaOVkfFNj-FnycijkbE
    
</br>

2- we will use the old Arduino arm model as our starting point. 

    catkin_%workspace name% -> src -> arduni_robot_arm -> robot_arm_pkg -> meshes -> stl
    
    
3- Delete all files then copy the 6 files downloaded from the drive that end with .stl extention.


4- Go to the folder urdf

    catkin_%workspace name% -> src -> arduni_robot_arm - > robot_arm_pkg -> urdf
    
5- Edit the .urdf file then replace it with the following text: 

  [document.txt](https://github.com/iaama5005/Arduino_Robot_Arm_V2_installation_guide/files/9332406/document.txt)

   
6- You need to remake the catkin file then run Rviz, Run these commands in cmd: 

    cd catkin_%workspace name%
    
    catkin_make
    
    source /home/%user name%/catkin_%workspace name%/devel/setup.bash
    
    roslaunch robot_arm_pkg check_motors.launch

7 - And that's it you can now view the new robot Arm in Rviz and move it freely using the joint state publisher.



Done now Arduino Robot Arm Version 2 is installed.
  
