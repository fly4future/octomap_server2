Port of the ROS1 [octomap server](https://github.com/OctoMap/octomap_mapping) for ROS2.0 

#### Installation
1.  Firstly make sure you have [octomap](https://github.com/OctoMap/octomap.git) installed on your system 
  ```bash
  sudo apt-get install ros-galactic-octomap ros-galactic-octomap-msgs
  ```

2.  Next, clone this ros package to the appropriate ros2 workspace
  ```bash
  git clone https://github.com/fly4future/octomap_server2.git
  ```

#### Building
Use colcon to build the workspace
```bash
colcon build --symlink-install --packages-select octomap_server2
```

### Notes:
- The package is compiled using `c++17` with `-O3` optimization.
