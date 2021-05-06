# mapping_dataset_styria
Open mapping dataset of styria in Austria



## Requirements

Tested on Ubuntu 18.04, ROS Melodic


## Datafiles

Data captured:
- Ouster OS1 64
- IMU XSense MTI-630
- GPS Ublox_f9p

Bagfiles are available for download: 

Graz Inner City (walking):

https://artirobots.sharepoint.com/:u:/g/EW7NEasfPFNNqX6kgPSrSJ4B8ifLob0q7ta24_YgT0TgIA?e=ZVh2ry

Planned route: 

![Planned Route Inner City](https://github.com/ARTI-Robots/mapping_dataset_styria/blob/main/docs/gpx_design_inner_city.jpg?raw=true "Planned Route Inner City")

Graz Schlossberg (walking):

https://artirobots.sharepoint.com/:u:/g/EcF9BHIY421Kqhf3DT4BxrkBhQt_U97iKyOeN4o3fx0hYA?e=E0iIqG

Graz Stadtpark (walking):

Cooming soon!

Planned route: 

![Planned Route Stadtpark](https://github.com/ARTI-Robots/mapping_dataset_styria/blob/main/docs/gpx_design_park.jpg?raw=true "Planned Route Stadtpark")

Vehicle Recordings

Cooming soon!


## Installation

```
cd ~/mapping_ws/src
git clone https://github.com/ARTI-Robots/mapping_dataset_styria.git
git clone https://github.com/virtual-vehicle-research/ouster_example.git
cd ..
catkin build
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





