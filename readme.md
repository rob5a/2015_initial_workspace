# Workspace inital des projets

workspace ROS indigo initial des projets de robotiques

# repartir de 0 (ou d'une version a jour de ce dépot) 
- bootez sur la clef USB
- montez la partition ROS
- cd /opt/ros
*attention! sauvegardez bien vos travaux avant*
- rm -rf catkin_ws
- git clone https://github.com/rob5a/2015_initial_workspace.git catkin_ws
- cd $HOME/catkin_ws
- source /opt/ros/indigo/setup.bash
- catkin build


# ajouter un dépot extérieur

par exemple : ardrone_tutorials de Mike Hamer (déja dans le ws initial!) 

$ cd $HOME/catkin_ws/src

$ git clone https://github.com/mikehamer/ardrone_tutorials.git

On vérifie que tout fonctionne ( que la branche master est bien la bonne! )

$ cd $HOME/catkin_ws

$ catkin build

On fige le repository en l'integrant a celui du projet

$ rm -rf ardrone_tutorials/.git

$ git add $HOME/catkin_ws/src/ardrone_tutorials

On explique pourquoi on utilise ce package :

$ git commit -am "ajout du package ros ardrone_tutorial pour apprendre a utiliser ardrone"

$ git push  origin master





