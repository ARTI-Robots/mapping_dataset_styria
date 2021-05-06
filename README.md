# mapping_dataset_styria
Open mapping dataset of styria in Austria



## Requirements

Tested on Ubuntu 18.04, ROS Melodic


## Datafiles

Bagfiles are available for download: 

Graz Inner City:
https://artirobots.sharepoint.com/:u:/g/EW7NEasfPFNNqX6kgPSrSJ4B8ifLob0q7ta24_YgT0TgIA?e=ZVh2ry

Graz Schlossberg:
https://artirobots.sharepoint.com/:u:/g/EcF9BHIY421Kqhf3DT4BxrkBhQt_U97iKyOeN4o3fx0hYA?e=E0iIqG

Cooming soon:
- Graz Stadtpark


## Installation

```
cd ~/mapping_ws/src
git clone https://github.com/ARTI-Robots/mapping_dataset_styria.git
git clone https://github.com/virtual-vehicle-research/ouster_example.git
cd ..
catkin build
```



## Run the package

```
roscore
```


```
roslaunch mapping_dataset_styria replay_vehicle.launch 
```

```
roslaunch mapping_dataset_styria replay_mapping_plattform.launch
```

```
rosbag play ROSBAG.bag --clock
```





