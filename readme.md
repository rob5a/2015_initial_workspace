# Workspace inital des projets

workspace ROS indigo initial des projets de robotiques

pour repartir de 0 (ou d'une version a jour de ce dépot) :
- bootez sur la clef USB
- montez la partition ROS
- cd /opt/ros
- rm -rf catkin_ws
- git clone https://github.com/rob5a/2015_initial_workspace.git catkin_ws
- cd $HOME/catkin_ws
- source /opt/ros/indigo/setup.bash
- catkin build
