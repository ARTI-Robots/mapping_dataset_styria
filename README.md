# mapping_dataset_styria
Open mapping dataset of styria in Austria



## Requirements

https://github.com/TixiaoShan/LIO-SAM/#dependency



## Installation

```
cd ~/mapping_ws/src
git clone https://github.com/ARTI-Robots/mapping_dataset_styria.git
git clone https://github.com/virtual-vehicle-research/ouster_example.git
git clone https://github.com/TixiaoShan/LIO-SAM.git
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
rosbag play ROSBAG.bag --clock -r 1.0
```



```
roslaunch mapping_dataset_styria lio_sam_vehicle.launch 
```





