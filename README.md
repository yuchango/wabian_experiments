# wabian_experiments
Datasets for walking experiments with the robotic platform WABIAN-2R

We generated one walking pattern for each step length with a fixed total walking distance of 1.5 m on a straight line. Step lengths are 0.10, 0.125, 0.15, 0.175, 0.2, 0.225 and 0.25 m. 
The reference walking cadence was fixed to 0.96 s/step, 0.06 seconds for double support phase and 0.9 seconds for single support phase. % (32 phases of 30 [ms] per step).
All patterns were executed on the robot by joint position control without any state estimation (i.e. assuming the reference trajectory of the base was executed perfectly). The motion capture and robot's joints, force, IMU and image data were stored and later analyzed

The datasets are diveded by step length (sl). Inside each step length folder there are three subfolders:
* *ROS_bags*: The robot sensor data was saved as rosbags, which contain the camera images and IMU data.
* *pattern*: The response csv files contain the data from each joint encoder (*\*\_jt.csv*), as well as the data from the force/torque sensors mounted on the robot's feet (*\*\_jr.csv*).
* *mocap*: The ground truth csv files contain the position and orientation data from the camera rigid body, as well as the position from each of the markers.



The datasets can be found in the following link:
https://drive.google.com/drive/folders/1n8to_4acDg6YZEMJ1_H0k4SodmGWwdXX?usp=sharing
