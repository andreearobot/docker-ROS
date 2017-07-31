
# docker-ROS
Docker images for using  ROS in Robots based in Raspberry Pi SBC

These images are built on top of esteve/ros:kinetic-robot-armhf

   * **Dockerfile** in folder *kinetic-robot-armhf* -> ROS Kinetic for ARMHF devices

      - BUILD THE IMAGE:
```
$ docker build -t local/ros-catkin:kinetic-robot-armhf .
```
      - RUN A BASH SESSION:
```
$ docker run --name ros-kinetic -it local/ros-catkin:kinetic-robot-armhf
```

   * **Dockerfile** in folder *kinetic-jus_avoid* -> Robot JUS, package 'jus_avoid'. Try by running in the shell the command 'roslaunch jus_avoid avoid_obstacles'


      - BUILD THE IMAGE:
```
$ docker build -t local/ros-catkin:kinetic-jus_avoid .
```
      - RUN A BASH SESSION:
```
$ docker run --name ros-jus_avoid -d local/ros-catkin:kinetic-jus_avoid


Docker hub URL for pulling theses images is:

https://hub.docker.com/r/therobotacademy/ros-catkin/
