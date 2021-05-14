# Mapping Dataset Styria
Open mapping dataset of styria in Austria



## Requirements

Tested on Ubuntu 18.04/20.04 ROS Melodic/Noetic 


## Sensor setup for walking dataset

| Type | Sensor | Topic| Frequency |  
| ------ | ------ | ------ | ------ |
| Lidar | 1x Ouster OS1-64 | /lidar/points | 10Hz | 
| IMU | XSens MTi-630 | /imu/data | 400Hz  | 
| GPS | u-blox F9P | /ublox_f9p/fix | 1Hz | 



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

The demonstrator from Virtual Vehicle Research is equipped with multiple lidars and other sensors for the mapping. To reduce the amount of data only the top-mounted lidar on the vehicle was recorded for all ROSBAGs. One recording includes as well the front/left and right placed Lidars. A high-precision RTK-GPS from NovAtel was used for some recordings to have a ground truth for the positioning. 

| Type | Sensor | Topic| Frequency |  
| ------ | ------ | ------ | ------ |
| Lidar | 1x Ouster OS2-128 | /lidar_top/points | 10Hz | 
| IMU | XSens MTi-630 | /sensing/imu/imu_data | >=200Hz  | 
| GPS | u-blox F9P | /sensing/ublox_f9p/fix  /sensing/ublox_f9p/speed | 5Hz | 
| Lidar (optional) | 3x Ouster OS0-64 | /lidar_front/points /lidar_middle_left/points /lidar_middle_right/points | 10Hz | 
| GPS (optional) | NovAtel ProPak6 | /sensing/novatel/fix | 100Hz |




![alt text](https://github.com/ARTI-Robots/mapping_dataset_styria/blob/main/docs/vehicle_sensor_positions.png?raw=true)


### Graz University of Technology Campus (driving, low speed):

**Duration:**    21:02s (1232s)  
**Size:**        29.5 GB  

![University Campus](https://github.com/ARTI-Robots/mapping_dataset_styria/blob/main/docs/1_university_campus.jpg?raw=true "University Campus")

university_campus_2021-01-25-15-59-55_0.zip  
https://v2c2.sharepoint.com/:u:/s/msteams_project-team_a6232st/EYY8Z-SuraJJntc1KN6JoqAB4kFQvc0VKSQBq-wZqi6lUQ?e=Vbm6c1   
university_campus_2021-01-25-16-14-56_1.zip  
https://v2c2.sharepoint.com/:u:/s/msteams_project-team_a6232st/EbW-cuGCy15Bnm5G7mHsi9EBrBWb0B9A6TziWNnmJmYb5w?e=DOkFAp


### Graz Inner City (driving):

**Duration:**    29:13s (1753s)  
**Size:**        49.3 GB  

![University Campus](https://github.com/ARTI-Robots/mapping_dataset_styria/blob/main/docs/6_campus_city_center_campus.jpg?raw=true "University Campus")

Uploading in progress!

### Urban Environment 1 (Graz University of Technology -> Murpark):

**Duration:**    10:06s (606s)  
**Size:**        9.9 GB  

![Urban environment 1](https://github.com/ARTI-Robots/mapping_dataset_styria/blob/main/docs/2_campus_murpark.jpg?raw=true "Urban environment 1")

campus_murpark_2021-03-16-16-27-02_0.zip  
https://v2c2.sharepoint.com/:u:/s/msteams_project-team_a6232st/EXiXlPWXwTBDni7krobKF7YBN1d6THEEux7I2fT8qPux7w?e=y23xBA  
campus_murpark_2021-03-16-16-30-00_1.zip  
https://v2c2.sharepoint.com/:u:/s/msteams_project-team_a6232st/ESV9n6LFv_NOtsZse4cJDZABgfhkUL3U1BWGIbdkfZXV-w?e=iAgYTq  
campus_murpark_2021-03-16-16-33-07_2.zip  
https://v2c2.sharepoint.com/:u:/s/msteams_project-team_a6232st/EQ9dDOPOx-pAkSNq0aIi8jwBEcl5Z0xfSt9GN79BtpHwLA?e=RVXeam  
campus_murpark_2021-03-16-16-36-13_3.zip  
https://v2c2.sharepoint.com/:u:/s/msteams_project-team_a6232st/EZJdS-YpAlZPtgvbyFEO2m8BQZMRFCwHd2yw3vs305NeWg?e=dcZaWb


### Motorway (Murpark -> A2 -> Murpark):

**Duration:**    12:18s (738s)  
**Size:**        10.2 GB  

![Motorway](https://github.com/ARTI-Robots/mapping_dataset_styria/blob/main/docs/3_murpark_a2_murpark.jpg?raw=true "University Campus")

murpark_a2_murpark_2021-03-16-16-37-19_0.zip   
https://v2c2.sharepoint.com/:u:/s/msteams_project-team_a6232st/ET3pY37xB0hJgrjeV400q5EB1ajXSDfW875tcvEzdJW4iw?e=kbBUDx  
murpark_a2_murpark_2021-03-16-16-40-27_1.zip  
https://v2c2.sharepoint.com/:u:/s/msteams_project-team_a6232st/EZu51bCyDLlGqeQYYJvxG1kB61-J5s9TbbLBYuo6TzymfQ?e=2mX6Oo  
murpark_a2_murpark_2021-03-16-16-43-26_2.zip  
https://v2c2.sharepoint.com/:u:/s/msteams_project-team_a6232st/EZUTXDD-IBhGrPgtGwfznF0BWl4d6BZpJw6q80hfAQlE2Q?e=0HdvhZ  
murpark_a2_murpark_2021-03-16-16-46-31_3.zip  
https://v2c2.sharepoint.com/:u:/s/msteams_project-team_a6232st/EYy5JDHWXdBDoaWhfufqnWoBVOhpLcKaMplGz7PerqqSCA?e=Uz7fZD



### Urban environment 2 (Murpark -> Graz University of Technology):

**Duration:**    06:04s (364s)  
**Size:**        5.4 GB  

![Urban environment 2](https://github.com/ARTI-Robots/mapping_dataset_styria/blob/main/docs/4_murpark_campus.jpg?raw=true "Urban environment 2")

murpark_campus_2021-03-16-17-26-26_0.zip  
https://v2c2.sharepoint.com/:u:/s/msteams_project-team_a6232st/EZVz2fplA0lIpQfTpk5THo0B1kdWCJvVsw8owEHQCGtA6A?e=LUPXRQ  
murpark_campus_2021-03-16-17-29-27_1.zip  
https://v2c2.sharepoint.com/:u:/s/msteams_project-team_a6232st/EdI-CAfcBKBAkuJScWNCIsYBfDl8REw-XoLTGZqlLfXkrQ?e=VakPSH


### 4x Lidars (Graz University of Technology Campus):

**Duration:**    18:44s (1124s)  
**Size:**        35.3 GB  

![Vehicle 4xLidar setup](https://github.com/ARTI-Robots/mapping_dataset_styria/blob/main/docs/vehicle_4_lidars.png?raw=true "Vehicle 4xLidar setup")

vehicle_4_lidars_2021-01-22-05-36-56_0.zip  
https://v2c2.sharepoint.com/:u:/s/msteams_project-team_a6232st/EUccCxSWKSZCtzg65ZyeSjIBrvjRLBfjdh44oNno9F19fw?e=gX1ZEw  
vehicle_4_lidars_2021-01-22-05-46-24_1.zip  
https://v2c2.sharepoint.com/:u:/s/msteams_project-team_a6232st/EQznXe0z351AndrMzUBBIOkBkSeRpHzmnJJyRuagFVvNug?e=2WWqIC  
vehicle_4_lidars_2021-01-22-05-55-41_2.zip  
https://v2c2.sharepoint.com/:u:/s/msteams_project-team_a6232st/EUkwtvFQFhBLsPaoEUDdlXoBdvf9EwAMMRkxbArNUiTUbQ?e=fi4TuT


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


