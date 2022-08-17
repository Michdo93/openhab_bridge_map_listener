# openhab_bridge_map_listener

ROS package which listens and subscribes to the map topic. This image will be published as command to openHAB using a bridge between openHAB and ROS with HABApp. 
## Installation

Go to the `catkin_ws/src` folder and clone the repository:

```
cd ~/catkin_ws/src
git clone https://github.com/Michdo93/openhab_bridge_map_listener.git
cd ~/catkin_ws
catkin_make
```

## Usage

At first you have to run a ROS program which publishes to the topic `map`. Equivalent to

```
rosrun map_server map_saver -f ~/map
```

you can now run:

```
rosrun openhab_bridge_map_listener mapListener.py
```
