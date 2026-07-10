# mvp-sightseeing-vehicle platform
## 1.Hardware
BOM: 

|  Material   |    Spec     |
| ----------- | ----------- |
| Computer    | MS-01       |
| Vehicle     | G4          |
| Lidar       | TM-32       |

## 2.Enviroment:
  (1) Ubuntu 20.04
  (2) ROS1 noetic
  (3) Docker
  
## 3.Framework:
### 3.1 Autoware.ai-mvp
### 3.1.1 Pointcloud Scheme
  （1）SLAM：ndt_mapping
  （2）Localization: ndt_matching
  （3）global planner: record path
  （4）local planner: astar_avoid+velocity_set
  （5）control: pure pursuit
#### 3.1.2 HD-Map Scheme
  （1）SLAM：HD-Map tools
  （2）Localization: ndt_matching
  （3）global planner: dp
  （4）local planner: openplanner
  （5）control: pure pursuit
  
### 3.2 neupan_cpp
  （1）SLAM：fastlio2
  （2）Localization: fastlio2
  （3）global planner: record path
  （4）local planner: neupan
  （5）control: pure pursuit
