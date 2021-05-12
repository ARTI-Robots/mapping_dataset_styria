# Mapping Dataset Styria
Open mapping dataset of styria in Austria



## Requirements

Tested on Ubuntu 18.04/20.04 ROS Melodic/Noetic 


## Datafiles

Data captured:
- Ouster OS1 64
- IMU XSense MTI-630
- GPS Ublox_f9p

Bagfiles are available for download below. 

#### Graz Inner City (walking):

Duration:    29:07s (1747s)  
Size:        27.0 GB  

inner_city.zip  
https://artirobots.sharepoint.com/:u:/g/EW7NEasfPFNNqX6kgPSrSJ4B8ifLob0q7ta24_YgT0TgIA?e=ZVh2ry

Planned route: 

![Planned Route Inner City](https://github.com/ARTI-Robots/mapping_dataset_styria/blob/main/docs/gpx_design_inner_city.jpg?raw=true "Planned Route Inner City")

#### Graz Schlossberg (walking):

Duration:    32:57s (1977s)  
Size:        30.5 GB  

schlossberg.zip  
https://artirobots.sharepoint.com/:u:/g/EcF9BHIY421Kqhf3DT4BxrkBhQt_U97iKyOeN4o3fx0hYA?e=E0iIqG

#### Graz Stadtpark (walking):

Duration:    51:50s (3110s)  
Size:        48.0 GB  

park.zip  
https://artirobots.sharepoint.com/:u:/g/EdIVjOiqYhtMgHvKGAZlkRgBDvNG04Al-CjxZWe8sQg4yg?e=A96ck7

Planned route: 

![Planned Route Stadtpark](https://github.com/ARTI-Robots/mapping_dataset_styria/blob/main/docs/gpx_design_park.jpg?raw=true "Planned Route Stadtpark")

## Vehicle Recordings by Virtual Vehicle Research

The demonstrator from Virtual Vehicle Research is equipped with differant type of sensors. For the mapping dataset sensors in the table below are used. To reduce the amout of data only the Lidar on the top of the vehicle was recorded all the time. Some recordings include as well the front/left and right placed Lidars. 
To have a ground truth reference for some recordings a high-precision RTK-GPS from NovAtel was used for some recordings.

| Type | Sensor | Topic| Frequency |  
| ------ | ------ | ------ | ------ |
| Lidar | 1x Ouster OS0-128 | /lidar_top/points | 10Hz | 
| IMU | XSens MTi-630 | /sensing/imu/imu_data | >=200Hz  | 
| GPS | u-blox F9P | /sensing/ublox_f9p/fix  /sensing/ublox_f9p/speed | 5Hz | 
| Lidar (optional) | 3x Ouster OS2-64 | /lidar_front/points /lidar_middle_left/points /lidar_middle_right/points | 10Hz | 
| GPS (optional) | NovAtel ProPak6 | /sensing/novatel/fix | 100Hz |




![alt text](https://github.com/ARTI-Robots/mapping_dataset_styria/blob/main/docs/vehicle_sensor_positions.png?raw=true)


### Graz University of Technology

**Duration:**    21:02s (1232s)  
**Size:**        29.5 GB  



![University Campus](https://github.com/ARTI-Robots/mapping_dataset_styria/blob/main/docs/1_university_campus.jpg?raw=true "University Campus")

[university_campus_2021-01-25-15-59-55_0.zip ](https://v2c2.sharepoint.com/:u:/s/msteams_project-team_a6232st/EYY8Z-SuraJJntc1KN6JoqAB4kFQvc0VKSQBq-wZqi6lUQ?e=Vbm6c1) 

[university_campus_2021-01-25-16-14-56_1.zip](https://v2c2.sharepoint.com/:u:/s/msteams_project-team_a6232st/EbW-cuGCy15Bnm5G7mHsi9EBrBWb0B9A6TziWNnmJmYb5w?e=DOkFAp)  


### Graz University of Technology -> Murpark:

**Duration:**    10:06s (606s)  
**Size:**        00.0 GB  

![Planned Route Inner City](https://github.com/ARTI-Robots/mapping_dataset_styria/blob/main/docs/gpx_design_inner_city.jpg?raw=true "Planned Route Inner City")

[campus_murpark_2021-03-16-16-27-02_0.zip](https://v2c2.sharepoint.com/:u:/s/msteams_project-team_a6232st/Ebgl20XkaaZKplzmqWScY_UBDZJnIgRvkponp9HctTYUyQ?e=iXBdce)  

[campus_murpark_2021-03-16-16-30-00_1.zip ](https://v2c2.sharepoint.com/:u:/s/msteams_project-team_a6232st/EYHCdKCGcaVBvtzBFxo3-_sB9gL9jT6t8c8XAG_oWWyi8A?e=OM9Z4D) 

[campus_murpark_2021-03-16-16-33-07_2.zip](https://v2c2.sharepoint.com/:u:/s/msteams_project-team_a6232st/EdU6pX5b5GVBqsSXjwLPak0BnDKz9ik2qnjt-x4X2RVQRw?e=SJfL74)  

[campus_murpark_2021-03-16-16-36-13_3.zip](https://v2c2.sharepoint.com/:u:/s/msteams_project-team_a6232st/ESX4gSXBx2hOmrszrDWmQQkB2eD3ajASiv_GofXFpJxdjw?e=ycoivn)  




## Installation

```
cd ~/mapping_ws/src
git clone https://github.com/ARTI-Robots/mapping_dataset_styria.git
git clone https://github.com/virtual-vehicle-research/ouster_example.git
cd ..
catkin_make
```



## Run the package with mapping plattform (walking)

```
roscore
```

```
roslaunch mapping_dataset_styria replay_mapping_plattform.launch
```

```
rosbag play ROSBAG.bag --clock
```

## Run the package with vehicle plattform (driving)

```
roscore
```

```
roslaunch mapping_dataset_styria replay_vehicle.launch 
```

```
rosbag play ROSBAG.bag --clock
```

## Powered by

[ARTI - Autonomous Robot Technology GmbH](http://arti-robots.com)

[Virtual Vehicle Research GmbH](https://www.v2c2.at/)


