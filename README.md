Dedicated workspace for including all workspace environment variables, so as to solve the workspace overlaying problem.

- [catkin配置多工作空间-workspace_overlaying](https://blog.csdn.net/dndxjj/article/details/90712809)

- [Overlaying with catkin workspaces](http://wiki.ros.org/catkin/Tutorials/workspace_overlaying)

### Usage

- Add ``<your_ws>/devel`` to ``catkin_overlay_ws/devel/_setup_util.py`` line 271
```
CMAKE_PREFIX_PATH = r'/home/lyh/Codes/catkin_ws/devel;/home/lyh/Codes/robot_ws/devel;/home/lyh/Codes/calibration_ws/devel;/home/lyh/Codes/safety_hrc_ws/devel;/home/lyh/Codes/hri_ws/devel;/opt/ros/melodic'.split(';')
```

- Add ``source ~/Codes/catkin_overlay_ws/devel/setup.bash`` to ``~/.bashrc``

- Run ``source ~/.bashrc``