# install-robot-arm
# install source code
```bash
git clone https://github.com/smart-methods/arduino_robot_arm.git 
```
# Dependencies
- make sure you installed all these packages:
```bash
sudo apt-get install ros-noetic-catkin
```
- create folder
```bash
mkdir -p ~/catkin_ws/src
```
- go to the folder
```bash
cd ~/catkin_ws/
```
- Install arm package in folder
```bash
catkin_make
```
```bash
cd ~/catkin_ws/src
```
```bash
git clone https://github.com/smart-methods/arduino_robot_arm.git 
```
```bash
cd ~/catkin_ws
```
```bash
rosdep install --from-paths src --ignore-src -r -y
```
```bash
sudo apt-get install ros-kinetic-moveit
```
```bash
sudo apt-get install ros-kinetic-joint-state-publisher ros-kinetic-joint-state-publisher-gui
```
```bash
sudo apt-get install ros-kinetic-gazebo-ros-control joint-state-publisher
```
```bash
sudo apt-get install ros-kinetic-ros-controllers ros-kinetic-ros-control
```
- go to file (bashrc)
```bash
sudo nano ~/.bashrc
```
- at the end of the (bashrc) file add the follwing line
```bash
source /home/raghad/catkin_ws/devel/setup.bash
```
- then ctrl + o >> enter>> ctrl + x (to go out)
- update  the file
```bash
source ~/.bashrc
```
- open the RIVZ
```pash
roslaunch robot_arm_pkg check_motors.launch
```
# Testing
![Screenshot from 2022-07-24 01-56-51 (2)](https://user-images.githubusercontent.com/109127124/180652889-06723cf5-67de-487f-856a-6d637e9f97e9.png)
![Screenshot from 2022-07-24 01-57-27](https://user-images.githubusercontent.com/109127124/180652935-1d78e87a-8f17-4d98-81c6-576d66fbc066.png)
![Screenshot from 2022-07-24 01-58-39](https://user-images.githubusercontent.com/109127124/180652977-6d85d182-2056-4873-914c-9faa3f75efa7.png)





