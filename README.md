# clicksight

Collection of github repositories used to faciliate simple and efficient robot workspace setup. 

##  Main system components

System for easy robot workspace setup consists of: 
* motion capture system 
* kalipen 
* robot arm 

## Prerequisites

- PC with bluetooth 
- Linux xyz
- Optitrack mocap system

## Init repository 

After cloning repository, run: 
```
git submodule update --remote 
```
to fetch newest updates to the system. 

## Robot arm setup: 

In order to start robot arm, you first need to build docker image for the robot manipulation. 
To do so, after updating git submodules, run following commands: 
```
cd ./ros-noetic/for_course_lab/or2324
docker build -t for_img . 
```

After image is sucessfuly built, you can run it with:
```
./first_run.sh
```

## TODO: 
- [ ] [arm control] Develop arm control for following straight paths
- [x] [kalipen] Test kalipen functionality 
- [x] [perception] Scan matching algorithm to setup STL 
- [x] [perception] Draw obstacles
- [ ] [perception] Test scan matching
- [ ] [docs] Add docs for using the system 
- [ ] [docs] How to run optitrack 
- [ ] [docs] How to run kalipen 
- [ ] [docs] How to run robot arm 

