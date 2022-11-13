# Multi-Robot-Formation-Control

A **group project** implemented in February 2020 for the third year Mobile Robot Systems course at the University of Cambridge

The project report can be found at: `report.pdf`

The results of the project can be found in a video I compiled (`MultiRobotFormationControl.mp4`)

An overview of the project work can be found in the presentation `MultiRobotFormationControl.pptx`.

## Requirements
```
cd src_directory_of_workspace
$ git clone https://github.com/ROBOTIS-GIT/turtlebot3.git

$ git clone https://github.com/ROBOTIS-GIT/turtlebot3_simulations.git

$ git clone https://github.com/ROBOTIS-GIT/turtlebot3_msgs.git
```

## To Run
- Launch [Gazebo](http://gazebosim.org) using the environment you wish (e.g roslaunch package_name simple_column.launch)
- Go to init_formations.py and set MAP_PARAMS to the map you want (e.g SIMPLE_MAP)
- If you want to run RRT, set RUN_RRT to True
- Predefined paths are stored in the precomputed_rrt_paths.py file
- run formation_move.launch: roslaunch package_name formation_move.launch
*NOTE: If you change the starting positions of the robots in the environment, you need to recompute a new path, then either store it in the precomputed paths file or reset the starting positions*

To run the decentralised version, start any map as usual then launch formation_move_decentralized.launch for each robot, supplying id as an arg (e.g id:=1)

*Project contributors: Benjamin Philps (BenjaminPhi5), Sumaiyah Kola (sumaiyah) and Ajay Ahir (DoodleBobBuffPants)* 
