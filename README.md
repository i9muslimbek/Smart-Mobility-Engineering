# Smart-Mobility-Engineering-Lab
## Turtlesim: Installation
```
muslimjon@ubuntu:~$  sudo apt update
[sudo] password for muslimjon: 
Ign:1 cdrom://Ubuntu 20.04.5 LTS _Focal Fossa_ - Release amd64 (20220831) focal InRelease
Err:2 cdrom://Ubuntu 20.04.5 LTS _Focal Fossa_ - Release amd64 (20220831) focal Release
  Please use apt-cdrom to make this CD-ROM recognized by APT. apt-get update cannot be used to add new CD-ROMs
Ign:3 http://packages.ros.org/ros/ubuntu $(lsb_release InRelease
Hit:4 http://packages.ros.org/ros2/ubuntu focal InRelease                     
Err:5 http://packages.ros.org/ros/ubuntu $(lsb_release Release                
  404  Not Found [IP: 64.50.236.52 80]
Hit:6 http://archive.linux.duke.edu/ubuntu focal InRelease                    
Get:7 http://packages.ros.org/ros/ubuntu focal InRelease [4,679 B]            
Get:8 http://archive.linux.duke.edu/ubuntu focal-updates InRelease [114 kB]   
Err:7 http://packages.ros.org/ros/ubuntu focal InRelease                
  The following signatures couldn't be verified because the public key is not available: NO_PUBKEY F42ED6FBAB17C654
Hit:9 http://archive.linux.duke.edu/ubuntu focal-backports InRelease          
Hit:10 http://archive.canonical.com/ubuntu xenial InRelease                   
Get:11 http://archive.linux.duke.edu/ubuntu focal-security InRelease [114 kB]
Hit:12 http://archive.linux.duke.edu/ubuntu focal-proposed InRelease          
Get:13 http://archive.linux.duke.edu/ubuntu focal-updates/main amd64 DEP-11 Metadata [277 kB]
Get:14 http://archive.linux.duke.edu/ubuntu focal-updates/universe amd64 DEP-11 Metadata [391 kB]
Get:15 http://archive.linux.duke.edu/ubuntu focal-updates/multiverse amd64 DEP-11 Metadata [944 B]
Get:16 http://archive.linux.duke.edu/ubuntu focal-security/main amd64 DEP-11 Metadata [40.7 kB]
Get:17 http://archive.linux.duke.edu/ubuntu focal-security/universe amd64 DEP-11 Metadata [77.4 kB]
Get:18 http://archive.linux.duke.edu/ubuntu focal-security/multiverse amd64 DEP-11 Metadata [2,464 B]
Reading package lists... Done                             E: The repository 'cdrom://Ubuntu 20.04.5 LTS _Focal Fossa_ - Release amd64 (20220831) focal Release' does not have a Release file.
N: Updating from such a repository can't be done securely, and is therefore disabled by default.
N: See apt-secure(8) manpage for repository creation and user configuration details.
E: The repository 'http://packages.ros.org/ros/ubuntu $(lsb_release Release' does not have a Release file.
N: Updating from such a repository can't be done securely, and is therefore disabled by default.
N: See apt-secure(8) manpage for repository creation and user configuration details.
W: Target Sources (main/source/Sources) is configured multiple times in /etc/apt/sources.list:2 and /etc/apt/sources.list:7
W: GPG error: http://packages.ros.org/ros/ubuntu focal InRelease: The following signatures couldn't be verified because the public key is not available: NO_PUBKEY F42ED6FBAB17C654
E: The repository 'http://packages.ros.org/ros/ubuntu focal InRelease' is not signed.
N: Updating from such a repository can't be done securely, and is therefore disabled by default.
N: See apt-secure(8) manpage for repository creation and user configuration details.
W: Target Sources (main/source/Sources) is configured multiple times in /etc/apt/sources.list:2 and /etc/apt/sources.list:7
muslimjon@ubuntu:~$ sudo apt install ros-rolling-turtlesim
Reading package lists... Done
Building dependency tree       
Reading state information... Done
ros-rolling-turtlesim is already the newest version (1.4.1-1focal.20220122.081255).
0 upgraded, 0 newly installed, 0 to remove and 0 not upgraded.
muslimjon@ubuntu:~$ ros2 pkg executables turtlesim
turtlesim draw_square
turtlesim mimic
turtlesim turtle_teleop_key
turtlesim turtlesim_node
muslimjon@ubuntu:~$ 
```
## Turtlesim: Start Turtlesim
```
muslimjon@ubuntu:~$  ros2 run turtlesim turtlesim_node
[INFO] [1665467714.914460392] [turtlesim]: Starting turtlesim with node name /turtlesim
[INFO] [1665467714.925839713] [turtlesim]: Spawning turtle [turtle1] at x=[5.544445], y=[5.544445], theta=[0.000000]

```
![Screenshot from 2022-10-10 22-56-35](https://user-images.githubusercontent.com/114977921/195008179-cfdb2d47-51ca-4f37-a01f-dc1ca373efc8.png)

## Turtlesim: Using Turtlesim
```
muslimjon@ubuntu:~$ ros2 run turtlesim turtle_teleop_key
Reading from keyboard
---------------------------
Use arrow keys to move the turtle.
Use G|B|V|C|D|E|R|T keys to rotate to absolute orientations. 'F' to cancel a rotation.
'Q' to quit.

```
![Screenshot from 2022-10-10 23-08-41](https://user-images.githubusercontent.com/114977921/195009735-2affd0ab-1e8f-4863-b8a5-8e8f652c7252.png)

## ROS2&RQT
### ROS2 Intallation
 ```
 muslimjon@ubuntu:~$  sudo apt update
[sudo] password for muslimjon: 
Ign:1 cdrom://Ubuntu 20.04.5 LTS _Focal Fossa_ - Release amd64 (20220831) focal InRelease
Err:2 cdrom://Ubuntu 20.04.5 LTS _Focal Fossa_ - Release amd64 (20220831) focal Release
  Please use apt-cdrom to make this CD-ROM recognized by APT. apt-get update cannot be used to add new CD-ROMs
Ign:3 http://packages.ros.org/ros/ubuntu $(lsb_release InRelease              
Get:4 http://packages.ros.org/ros/ubuntu focal InRelease [4,679 B]            
Err:4 http://packages.ros.org/ros/ubuntu focal InRelease                      
  The following signatures couldn't be verified because the public key is not available: NO_PUBKEY F42ED6FBAB17C654
Hit:5 http://packages.ros.org/ros2/ubuntu focal InRelease                     
Hit:6 http://archive.canonical.com/ubuntu xenial InRelease                    
Hit:7 http://archive.linux.duke.edu/ubuntu focal InRelease          
Err:8 http://packages.ros.org/ros/ubuntu $(lsb_release Release
  404  Not Found [IP: 64.50.236.52 80]
Get:9 http://archive.linux.duke.edu/ubuntu focal-updates InRelease [114 kB]
Get:10 http://archive.linux.duke.edu/ubuntu focal-backports InRelease [108 kB]
Get:11 http://archive.linux.duke.edu/ubuntu focal-security InRelease [114 kB] 
Get:12 http://archive.linux.duke.edu/ubuntu focal-proposed InRelease [267 kB] 
0% [12 InRelease 249 kB/267 kB 93%]                                                                                                                         Get:13 http://archive.linux.duke.edu/ubuntu focal-updates/restricted Sources [44.8 kB]
Get:14 http://archive.linux.duke.edu/ubuntu focal-updates/universe Sources [263 kB]
Get:15 http://archive.linux.duke.edu/ubuntu focal-updates/main Sources [527 kB]    
Get:16 http://archive.linux.duke.edu/ubuntu focal-updates/main amd64 Packages [2,191 kB]
Get:17 http://archive.linux.duke.edu/ubuntu focal-updates/main i386 Packages [744 kB]
Get:18 http://archive.linux.duke.edu/ubuntu focal-updates/main Translation-en [385 kB]
Get:19 http://archive.linux.duke.edu/ubuntu focal-updates/main amd64 DEP-11 Metadata [277 kB]
Get:20 http://archive.linux.duke.edu/ubuntu focal-updates/main amd64 c-n-f Metadata [16.0 kB]
Get:21 http://archive.linux.duke.edu/ubuntu focal-updates/restricted i386 Packages [26.6 kB]
Get:22 http://archive.linux.duke.edu/ubuntu focal-updates/restricted amd64 Packages [1,367 kB]
Get:23 http://archive.linux.duke.edu/ubuntu focal-updates/restricted Translation-en [193 kB]
Get:24 http://archive.linux.duke.edu/ubuntu focal-updates/restricted amd64 c-n-f Metadata [592 B]
Get:25 http://archive.linux.duke.edu/ubuntu focal-updates/universe i386 Packages [697 kB]
Get:26 http://archive.linux.duke.edu/ubuntu focal-updates/universe amd64 Packages [970 kB]
Get:27 http://archive.linux.duke.edu/ubuntu focal-updates/universe Translation-en [221 kB]
Get:28 http://archive.linux.duke.edu/ubuntu focal-updates/universe amd64 DEP-11 Metadata [406 kB]
Get:29 http://archive.linux.duke.edu/ubuntu focal-updates/universe DEP-11 48x48 Icons [261 kB]
Get:30 http://archive.linux.duke.edu/ubuntu focal-updates/universe DEP-11 64x64 Icons [465 kB]
Get:31 http://archive.linux.duke.edu/ubuntu focal-updates/universe amd64 c-n-f Metadata [21.8 kB]
Get:32 http://archive.linux.duke.edu/ubuntu focal-updates/multiverse amd64 DEP-11 Metadata [940 B]
Get:33 http://archive.linux.duke.edu/ubuntu focal-backports/main amd64 DEP-11 Metadata [7,972 B]
Get:34 http://archive.linux.duke.edu/ubuntu focal-backports/universe amd64 DEP-11 Metadata [30.5 kB]
Get:35 http://archive.linux.duke.edu/ubuntu focal-security/universe Sources [111 kB]
Get:36 http://archive.linux.duke.edu/ubuntu focal-security/restricted Sources [44.7 kB]
Get:37 http://archive.linux.duke.edu/ubuntu focal-security/main Sources [251 kB]   
Get:38 http://archive.linux.duke.edu/ubuntu focal-security/main amd64 Packages [1,784 kB]
Get:39 http://archive.linux.duke.edu/ubuntu focal-security/main i386 Packages [508 kB]
Get:40 http://archive.linux.duke.edu/ubuntu focal-security/main Translation-en [297 kB]
Get:41 http://archive.linux.duke.edu/ubuntu focal-security/main amd64 DEP-11 Metadata [40.7 kB]
Get:42 http://archive.linux.duke.edu/ubuntu focal-security/main amd64 c-n-f Metadata [11.2 kB]
Get:43 http://archive.linux.duke.edu/ubuntu focal-security/restricted i386 Packages [25.3 kB]
Get:44 http://archive.linux.duke.edu/ubuntu focal-security/restricted amd64 Packages [1,241 kB]
Get:45 http://archive.linux.duke.edu/ubuntu focal-security/restricted Translation-en [176 kB]
Get:46 http://archive.linux.duke.edu/ubuntu focal-security/restricted amd64 c-n-f Metadata [596 B]
Get:47 http://archive.linux.duke.edu/ubuntu focal-security/universe i386 Packages [566 kB]
Get:48 http://archive.linux.duke.edu/ubuntu focal-security/universe amd64 Packages [739 kB]
Get:49 http://archive.linux.duke.edu/ubuntu focal-security/universe Translation-en [136 kB]
Get:50 http://archive.linux.duke.edu/ubuntu focal-security/universe amd64 DEP-11 Metadata [93.0 kB]
Get:51 http://archive.linux.duke.edu/ubuntu focal-security/universe DEP-11 48x48 Icons [41.2 kB]
Get:52 http://archive.linux.duke.edu/ubuntu focal-security/universe DEP-11 64x64 Icons [84.7 kB]
Get:53 http://archive.linux.duke.edu/ubuntu focal-security/universe amd64 c-n-f Metadata [15.3 kB]
Get:54 http://archive.linux.duke.edu/ubuntu focal-security/multiverse amd64 DEP-11 Metadata [2,464 B]
Get:55 http://archive.linux.duke.edu/ubuntu focal-proposed/universe i386 Packages [23.1 kB]
Get:56 http://archive.linux.duke.edu/ubuntu focal-proposed/universe amd64 Packages [39.9 kB]
Get:57 http://archive.linux.duke.edu/ubuntu focal-proposed/universe Translation-en [20.6 kB]
Get:58 http://archive.linux.duke.edu/ubuntu focal-proposed/universe amd64 DEP-11 Metadata [4,040 B]
Get:59 http://archive.linux.duke.edu/ubuntu focal-proposed/universe DEP-11 48x48 Icons [1,348 B]
Get:60 http://archive.linux.duke.edu/ubuntu focal-proposed/universe DEP-11 64x64 Icons [10.4 kB]
Get:61 http://archive.linux.duke.edu/ubuntu focal-proposed/universe amd64 c-n-f Metadata [2,180 B]
Get:62 http://archive.linux.duke.edu/ubuntu focal-proposed/main amd64 Packages [168 kB]
Get:63 http://archive.linux.duke.edu/ubuntu focal-proposed/main i386 Packages [38.7 kB]
Get:64 http://archive.linux.duke.edu/ubuntu focal-proposed/main Translation-en [38.5 kB]
Get:65 http://archive.linux.duke.edu/ubuntu focal-proposed/main amd64 DEP-11 Metadata [25.7 kB]
Get:66 http://archive.linux.duke.edu/ubuntu focal-proposed/main DEP-11 48x48 Icons [871 B]
Get:67 http://archive.linux.duke.edu/ubuntu focal-proposed/main DEP-11 64x64 Icons [869 B]
Get:68 http://archive.linux.duke.edu/ubuntu focal-proposed/main amd64 c-n-f Metadata [1,084 B]
Get:69 http://archive.linux.duke.edu/ubuntu focal-proposed/multiverse amd64 Packages [7,044 B]
Get:70 http://archive.linux.duke.edu/ubuntu focal-proposed/multiverse i386 Packages [9,512 B]
Get:71 http://archive.linux.duke.edu/ubuntu focal-proposed/multiverse Translation-en [4,860 B]
Get:72 http://archive.linux.duke.edu/ubuntu focal-proposed/multiverse amd64 c-n-f Metadata [316 B]
Get:73 http://archive.linux.duke.edu/ubuntu focal-proposed/restricted amd64 Packages [172 kB]
Get:74 http://archive.linux.duke.edu/ubuntu focal-proposed/restricted Translation-en [24.5 kB]
Get:75 http://archive.linux.duke.edu/ubuntu focal-proposed/restricted amd64 c-n-f Metadata [116 B]
Reading package lists... Done                                                      
E: The repository 'cdrom://Ubuntu 20.04.5 LTS _Focal Fossa_ - Release amd64 (20220831) focal Release' does not have a Release file.
N: Updating from such a repository can't be done securely, and is therefore disabled by default.
N: See apt-secure(8) manpage for repository creation and user configuration details.
W: GPG error: http://packages.ros.org/ros/ubuntu focal InRelease: The following signatures couldn't be verified because the public key is not available: NO_PUBKEY F42ED6FBAB17C654
E: The repository 'http://packages.ros.org/ros/ubuntu focal InRelease' is not signed.
N: Updating from such a repository can't be done securely, and is therefore disabled by default.
N: See apt-secure(8) manpage for repository creation and user configuration details.
E: The repository 'http://packages.ros.org/ros/ubuntu $(lsb_release Release' does not have a Release file.
N: Updating from such a repository can't be done securely, and is therefore disabled by default.
N: See apt-secure(8) manpage for repository creation and user configuration details.
W: Target Sources (main/source/Sources) is configured multiple times in /etc/apt/sources.list:2 and /etc/apt/sources.list:7
W: Target Sources (main/source/Sources) is configured multiple times in /etc/apt/sources.list:2 and /etc/apt/sources.list:7
muslimjon@ubuntu:~$ sudo apt install ~nros-rolling-rqt*
Reading package lists... Done
Building dependency tree       
Reading state information... Done
The following additional packages will be installed:
  pybind11-dev python3-rospkg ros-rolling-class-loader
  ros-rolling-console-bridge-vendor ros-rolling-cv-bridge
  ros-rolling-diagnostic-msgs ros-rolling-image-transport
  ros-rolling-keyboard-handler ros-rolling-lifecycle-msgs
  ros-rolling-message-filters ros-rolling-pluginlib ros-rolling-pybind11-vendor
  ros-rolling-python-qt-binding ros-rolling-qt-dotgraph ros-rolling-qt-gui
  ros-rolling-qt-gui-cpp ros-rolling-qt-gui-py-common ros-rolling-rcl-lifecycle
  ros-rolling-rclpy ros-rolling-ros-image-to-qimage ros-rolling-ros2bag
  ros-rolling-ros2cli ros-rolling-rosbag2 ros-rolling-rosbag2-compression
  ros-rolling-rosbag2-compression-zstd ros-rolling-rosbag2-cpp
  ros-rolling-rosbag2-interfaces ros-rolling-rosbag2-py
  ros-rolling-rosbag2-storage ros-rolling-rosbag2-storage-default-plugins
  ros-rolling-rosbag2-transport ros-rolling-sensor-msgs
  ros-rolling-shared-queues-vendor ros-rolling-sqlite3-vendor
  ros-rolling-tango-icons-vendor ros-rolling-tinyxml2-vendor
  ros-rolling-yaml-cpp-vendor ros-rolling-zstd-vendor
Suggested packages:
  pybind11-doc
The following NEW packages will be installed:
  pybind11-dev python3-rospkg ros-rolling-class-loader
  ros-rolling-console-bridge-vendor ros-rolling-cv-bridge
  ros-rolling-diagnostic-msgs ros-rolling-image-transport
  ros-rolling-keyboard-handler ros-rolling-lifecycle-msgs
  ros-rolling-message-filters ros-rolling-pluginlib ros-rolling-pybind11-vendor
  ros-rolling-python-qt-binding ros-rolling-qt-dotgraph ros-rolling-qt-gui
  ros-rolling-qt-gui-cpp ros-rolling-qt-gui-py-common ros-rolling-rcl-lifecycle
  ros-rolling-rclpy ros-rolling-ros-image-to-qimage ros-rolling-ros2bag
  ros-rolling-ros2cli ros-rolling-rosbag2 ros-rolling-rosbag2-compression
  ros-rolling-rosbag2-compression-zstd ros-rolling-rosbag2-cpp
  ros-rolling-rosbag2-interfaces ros-rolling-rosbag2-py
  ros-rolling-rosbag2-storage ros-rolling-rosbag2-storage-default-plugins
  ros-rolling-rosbag2-transport ros-rolling-rqt ros-rolling-rqt-action
  ros-rolling-rqt-bag ros-rolling-rqt-bag-plugins ros-rolling-rqt-common-plugins
  ros-rolling-rqt-console ros-rolling-rqt-graph ros-rolling-rqt-gui
  ros-rolling-rqt-gui-cpp ros-rolling-rqt-gui-cpp-dbgsym ros-rolling-rqt-gui-py
  ros-rolling-rqt-image-overlay ros-rolling-rqt-image-overlay-dbgsym
  ros-rolling-rqt-image-overlay-layer ros-rolling-rqt-image-view
  ros-rolling-rqt-image-view-dbgsym ros-rolling-rqt-moveit ros-rolling-rqt-msg
  ros-rolling-rqt-plot ros-rolling-rqt-publisher ros-rolling-rqt-py-common
  ros-rolling-rqt-py-console ros-rolling-rqt-reconfigure
  ros-rolling-rqt-robot-dashboard ros-rolling-rqt-robot-monitor
  ros-rolling-rqt-robot-steering ros-rolling-rqt-runtime-monitor
  ros-rolling-rqt-service-caller ros-rolling-rqt-shell ros-rolling-rqt-srv
  ros-rolling-rqt-top ros-rolling-rqt-topic ros-rolling-sensor-msgs
  ros-rolling-shared-queues-vendor ros-rolling-sqlite3-vendor
  ros-rolling-tango-icons-vendor ros-rolling-tinyxml2-vendor
  ros-rolling-yaml-cpp-vendor ros-rolling-zstd-vendor
0 upgraded, 70 newly installed, 0 to remove and 27 not upgraded.
Need to get 13.3 MB of archives.
After this operation, 41.7 MB of additional disk space will be used.
Do you want to continue? [Y/n] y
Get:1 http://archive.linux.duke.edu/ubuntu focal/universe amd64 pybind11-dev all 2.4.3-2build2 [119 kB]
Get:2 http://packages.ros.org/ros2/ubuntu focal/main amd64 python3-rospkg all 1.4.0-100 [2,404 B]
Get:3 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-console-bridge-vendor amd64 1.3.2-1focal.20220120.195509 [15.1 kB]
Get:4 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-class-loader amd64 2.2.0-1focal.20220121.210047 [44.4 kB]
Get:5 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-sensor-msgs amd64 4.0.0-1focal.20220121.220001 [259 kB]
Get:6 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-cv-bridge amd64 3.0.2-2focal.20220127.230816 [112 kB]
Get:7 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-diagnostic-msgs amd64 4.0.0-1focal.20220121.222823 [80.3 kB]
Get:8 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-lifecycle-msgs amd64 1.1.0-1focal.20220121.213442 [97.3 kB]
Get:9 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rcl-lifecycle amd64 5.0.1-1focal.20220122.071811 [26.7 kB]
Get:10 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rclpy amd64 3.2.1-1focal.20220122.072501 [282 kB]
Get:11 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-message-filters amd64 4.2.0-1focal.20220122.080945 [36.5 kB]
Get:12 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-tinyxml2-vendor amd64 0.7.4-1focal.20220120.181059 [6,504 B]
Get:13 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-pluginlib amd64 5.1.0-1focal.20220121.210530 [27.9 kB]
Get:14 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-image-transport amd64 3.1.2-1focal.20220122.081507 [389 kB]
Get:15 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-keyboard-handler amd64 0.0.3-2focal.20220120.194622 [29.1 kB]
Get:16 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-pybind11-vendor amd64 2.3.0-1focal.20220120.180711 [5,372 B]
Get:17 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-python-qt-binding amd64 1.1.1-1focal.20220120.195235 [16.2 kB]
Get:18 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-qt-dotgraph amd64 2.1.1-1focal.20220120.195537 [15.2 kB]
Get:19 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-tango-icons-vendor amd64 0.1.0-3focal.20220120.195534 [5,580 B]
Get:20 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-qt-gui amd64 2.1.1-1focal.20220120.195819 [54.1 kB]
Get:21 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-qt-gui-cpp amd64 2.1.1-1focal.20220121.211623 [311 kB]
Get:22 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-qt-gui-py-common amd64 2.1.1-1focal.20220120.195538 [11.1 kB]
Get:23 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-ros-image-to-qimage amd64 0.0.2-1focal.20220127.231215 [10.7 kB]
Get:24 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-ros2cli amd64 0.17.1-1focal.20220126.184012 [38.5 kB]
Get:25 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-yaml-cpp-vendor amd64 8.0.0-1focal.20220204.185241 [152 kB]
Get:26 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rosbag2-storage amd64 0.13.0-1focal.20220204.185423 [166 kB]
Get:27 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-sqlite3-vendor amd64 0.13.0-1focal.20220120.180903 [7,416 B]
Get:28 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rosbag2-storage-default-plugins amd64 0.13.0-1focal.20220204.190125 [70.2 kB]
Get:29 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-shared-queues-vendor amd64 0.13.0-1focal.20220120.180849 [46.4 kB]
Get:30 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rosbag2-cpp amd64 0.13.0-1focal.20220204.190351 [206 kB]
Get:31 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rosbag2-compression amd64 0.13.0-1focal.20220204.191233 [132 kB]
Get:32 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rosbag2-interfaces amd64 0.13.0-1focal.20220121.214225 [96.8 kB]
Get:33 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rosbag2-transport amd64 0.13.0-1focal.20220204.192304 [262 kB]
Get:34 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rosbag2-py amd64 0.13.0-1focal.20220204.193524 [314 kB]
Get:35 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-ros2bag amd64 0.13.0-1focal.20220204.193831 [22.2 kB]
Get:36 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-zstd-vendor amd64 0.13.0-1focal.20220120.181332 [238 kB]
Get:37 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rosbag2-compression-zstd amd64 0.13.0-1focal.20220204.191850 [29.1 kB]
Get:38 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rosbag2 amd64 0.13.0-1focal.20220204.194704 [21.4 kB]
Get:39 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rqt-gui amd64 1.1.2-1focal.20220122.073030 [94.5 kB]
Get:40 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rqt-gui-cpp amd64 1.1.2-1focal.20220122.080244 [107 kB]
Get:41 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rqt-gui-py amd64 1.1.2-1focal.20220122.073306 [8,024 B]
Get:42 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rqt-py-common amd64 1.1.2-1focal.20220122.073039 [23.7 kB]
Get:43 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rqt amd64 1.1.2-1focal.20220122.083149 [6,888 B]
Get:44 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rqt-console amd64 2.0.2-1focal.20220122.073552 [48.8 kB]
Get:45 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rqt-msg amd64 1.0.5-1focal.20220122.073623 [13.7 kB]
Get:46 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rqt-action amd64 2.0.1-1focal.20220122.073654 [6,768 B]
Get:47 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rqt-bag amd64 1.1.1-1focal.20220204.193837 [79.3 kB]
Get:48 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rqt-plot amd64 1.1.1-1focal.20220122.073554 [40.6 kB]
Get:49 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rqt-bag-plugins amd64 1.1.1-1focal.20220204.194830 [24.1 kB]
Get:50 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rqt-graph amd64 1.2.1-1focal.20220122.073638 [40.4 kB]
Get:51 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rqt-image-view amd64 1.1.2-1focal.20220127.231213 [170 kB]
Get:52 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rqt-publisher amd64 1.1.3-1focal.20220122.073700 [22.2 kB]
Get:53 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rqt-py-console amd64 1.0.2-1focal.20220122.073554 [10.8 kB]
Get:54 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rqt-reconfigure amd64 1.0.8-1focal.20220122.073625 [45.1 kB]
Get:55 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rqt-service-caller amd64 1.0.5-1focal.20220122.073659 [15.3 kB]
Get:56 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rqt-shell amd64 1.0.2-1focal.20220122.073705 [13.6 kB]
Get:57 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rqt-srv amd64 1.0.3-1focal.20220122.073654 [6,704 B]
Get:58 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rqt-top amd64 1.0.2-1focal.20220122.073629 [12.0 kB]
Get:59 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rqt-topic amd64 1.2.2-1focal.20220122.073711 [18.8 kB]
Get:60 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rqt-common-plugins amd64 1.1.0-1focal.20220204.194902 [6,444 B]
Get:61 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rqt-gui-cpp-dbgsym amd64 1.1.2-1focal.20220122.080244 [2,168 kB]
Get:62 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rqt-image-overlay-layer amd64 0.0.2-1focal.20220131.224047 [7,248 B]
Get:63 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rqt-image-overlay amd64 0.0.2-1focal.20220131.224323 [139 kB]
Get:64 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rqt-image-overlay-dbgsym amd64 0.0.2-1focal.20220131.224323 [4,114 kB]
Get:65 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rqt-image-view-dbgsym amd64 1.1.2-1focal.20220127.231213 [2,162 kB]
Get:66 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rqt-moveit amd64 1.0.1-1focal.20220122.073739 [14.7 kB]
Get:67 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rqt-robot-monitor amd64 1.0.4-1focal.20220122.073557 [28.8 kB]
Get:68 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rqt-robot-dashboard amd64 0.6.1-1focal.20220122.073719 [51.4 kB]
Get:69 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rqt-robot-steering amd64 1.0.0-2focal.20220122.073610 [10.9 kB]
Get:70 http://packages.ros.org/ros2/ubuntu focal/main amd64 ros-rolling-rqt-runtime-monitor amd64 1.0.0-1focal.20220122.073621 [13.1 kB]
Fetched 13.3 MB in 1min 41s (132 kB/s)                                             
Extracting templates from packages: 100%
Selecting previously unselected package pybind11-dev.
(Reading database ... 246710 files and directories currently installed.)
Preparing to unpack .../00-pybind11-dev_2.4.3-2build2_all.deb ...
Unpacking pybind11-dev (2.4.3-2build2) ...
Selecting previously unselected package python3-rospkg.
Preparing to unpack .../01-python3-rospkg_1.4.0-100_all.deb ...
Unpacking python3-rospkg (1.4.0-100) ...
Selecting previously unselected package ros-rolling-console-bridge-vendor.
Preparing to unpack .../02-ros-rolling-console-bridge-vendor_1.3.2-1focal.20220120.1
95509_amd64.deb ...
Unpacking ros-rolling-console-bridge-vendor (1.3.2-1focal.20220120.195509) ...
Selecting previously unselected package ros-rolling-class-loader.
Preparing to unpack .../03-ros-rolling-class-loader_2.2.0-1focal.20220121.210047_amd
64.deb ...
Unpacking ros-rolling-class-loader (2.2.0-1focal.20220121.210047) ...
Selecting previously unselected package ros-rolling-sensor-msgs.
Preparing to unpack .../04-ros-rolling-sensor-msgs_4.0.0-1focal.20220121.220001_amd6
4.deb ...
Unpacking ros-rolling-sensor-msgs (4.0.0-1focal.20220121.220001) ...
Selecting previously unselected package ros-rolling-cv-bridge.
Preparing to unpack .../05-ros-rolling-cv-bridge_3.0.2-2focal.20220127.230816_amd64.
deb ...
Unpacking ros-rolling-cv-bridge (3.0.2-2focal.20220127.230816) ...
Selecting previously unselected package ros-rolling-diagnostic-msgs.
Preparing to unpack .../06-ros-rolling-diagnostic-msgs_4.0.0-1focal.20220121.222823_
amd64.deb ...
Unpacking ros-rolling-diagnostic-msgs (4.0.0-1focal.20220121.222823) ...
Selecting previously unselected package ros-rolling-lifecycle-msgs.
Preparing to unpack .../07-ros-rolling-lifecycle-msgs_1.1.0-1focal.20220121.213442_a
md64.deb ...
Unpacking ros-rolling-lifecycle-msgs (1.1.0-1focal.20220121.213442) ...
Selecting previously unselected package ros-rolling-rcl-lifecycle.
Preparing to unpack .../08-ros-rolling-rcl-lifecycle_5.0.1-1focal.20220122.071811_am
d64.deb ...
Unpacking ros-rolling-rcl-lifecycle (5.0.1-1focal.20220122.071811) ...
Selecting previously unselected package ros-rolling-rclpy.
Preparing to unpack .../09-ros-rolling-rclpy_3.2.1-1focal.20220122.072501_amd64.deb 
...
Unpacking ros-rolling-rclpy (3.2.1-1focal.20220122.072501) ...
Selecting previously unselected package ros-rolling-message-filters.
Preparing to unpack .../10-ros-rolling-message-filters_4.2.0-1focal.20220122.080945_
amd64.deb ...
Unpacking ros-rolling-message-filters (4.2.0-1focal.20220122.080945) ...
Selecting previously unselected package ros-rolling-tinyxml2-vendor.
Preparing to unpack .../11-ros-rolling-tinyxml2-vendor_0.7.4-1focal.20220120.181059_
amd64.deb ...
Unpacking ros-rolling-tinyxml2-vendor (0.7.4-1focal.20220120.181059) ...
Selecting previously unselected package ros-rolling-pluginlib.
Preparing to unpack .../12-ros-rolling-pluginlib_5.1.0-1focal.20220121.210530_amd64.
deb ...
Unpacking ros-rolling-pluginlib (5.1.0-1focal.20220121.210530) ...
Selecting previously unselected package ros-rolling-image-transport.
Preparing to unpack .../13-ros-rolling-image-transport_3.1.2-1focal.20220122.081507_
amd64.deb ...
Unpacking ros-rolling-image-transport (3.1.2-1focal.20220122.081507) ...
Selecting previously unselected package ros-rolling-keyboard-handler.
Preparing to unpack .../14-ros-rolling-keyboard-handler_0.0.3-2focal.20220120.194622
_amd64.deb ...
Unpacking ros-rolling-keyboard-handler (0.0.3-2focal.20220120.194622) ...
Selecting previously unselected package ros-rolling-pybind11-vendor.
Preparing to unpack .../15-ros-rolling-pybind11-vendor_2.3.0-1focal.20220120.180711_
amd64.deb ...
Unpacking ros-rolling-pybind11-vendor (2.3.0-1focal.20220120.180711) ...
Selecting previously unselected package ros-rolling-python-qt-binding.
Preparing to unpack .../16-ros-rolling-python-qt-binding_1.1.1-1focal.20220120.19523
5_amd64.deb ...
Unpacking ros-rolling-python-qt-binding (1.1.1-1focal.20220120.195235) ...
Selecting previously unselected package ros-rolling-qt-dotgraph.
Preparing to unpack .../17-ros-rolling-qt-dotgraph_2.1.1-1focal.20220120.195537_amd6
4.deb ...
Unpacking ros-rolling-qt-dotgraph (2.1.1-1focal.20220120.195537) ...
Selecting previously unselected package ros-rolling-tango-icons-vendor.
Preparing to unpack .../18-ros-rolling-tango-icons-vendor_0.1.0-3focal.20220120.1955
34_amd64.deb ...
Unpacking ros-rolling-tango-icons-vendor (0.1.0-3focal.20220120.195534) ...
Selecting previously unselected package ros-rolling-qt-gui.
Preparing to unpack .../19-ros-rolling-qt-gui_2.1.1-1focal.20220120.195819_amd64.deb
 ...
Unpacking ros-rolling-qt-gui (2.1.1-1focal.20220120.195819) ...
Selecting previously unselected package ros-rolling-qt-gui-cpp.
Preparing to unpack .../20-ros-rolling-qt-gui-cpp_2.1.1-1focal.20220121.211623_amd64
.deb ...
Unpacking ros-rolling-qt-gui-cpp (2.1.1-1focal.20220121.211623) ...
Selecting previously unselected package ros-rolling-qt-gui-py-common.
Preparing to unpack .../21-ros-rolling-qt-gui-py-common_2.1.1-1focal.20220120.195538
_amd64.deb ...
Unpacking ros-rolling-qt-gui-py-common (2.1.1-1focal.20220120.195538) ...
Selecting previously unselected package ros-rolling-ros-image-to-qimage.
Preparing to unpack .../22-ros-rolling-ros-image-to-qimage_0.0.2-1focal.20220127.231
215_amd64.deb ...
Unpacking ros-rolling-ros-image-to-qimage (0.0.2-1focal.20220127.231215) ...
Selecting previously unselected package ros-rolling-ros2cli.
Preparing to unpack .../23-ros-rolling-ros2cli_0.17.1-1focal.20220126.184012_amd64.d
eb ...
Unpacking ros-rolling-ros2cli (0.17.1-1focal.20220126.184012) ...
Selecting previously unselected package ros-rolling-yaml-cpp-vendor.
Preparing to unpack .../24-ros-rolling-yaml-cpp-vendor_8.0.0-1focal.20220204.185241_
amd64.deb ...
Unpacking ros-rolling-yaml-cpp-vendor (8.0.0-1focal.20220204.185241) ...
Selecting previously unselected package ros-rolling-rosbag2-storage.
Preparing to unpack .../25-ros-rolling-rosbag2-storage_0.13.0-1focal.20220204.185423
_amd64.deb ...
Unpacking ros-rolling-rosbag2-storage (0.13.0-1focal.20220204.185423) ...
Selecting previously unselected package ros-rolling-sqlite3-vendor.
Preparing to unpack .../26-ros-rolling-sqlite3-vendor_0.13.0-1focal.20220120.180903_
amd64.deb ...
Unpacking ros-rolling-sqlite3-vendor (0.13.0-1focal.20220120.180903) ...
Selecting previously unselected package ros-rolling-rosbag2-storage-default-plugins.
Preparing to unpack .../27-ros-rolling-rosbag2-storage-default-plugins_0.13.0-1focal
.20220204.190125_amd64.deb ...
Unpacking ros-rolling-rosbag2-storage-default-plugins (0.13.0-1focal.20220204.190125
) ...
Selecting previously unselected package ros-rolling-shared-queues-vendor.
Preparing to unpack .../28-ros-rolling-shared-queues-vendor_0.13.0-1focal.20220120.1
80849_amd64.deb ...
Unpacking ros-rolling-shared-queues-vendor (0.13.0-1focal.20220120.180849) ...
Selecting previously unselected package ros-rolling-rosbag2-cpp.
Preparing to unpack .../29-ros-rolling-rosbag2-cpp_0.13.0-1focal.20220204.190351_amd
64.deb ...
Unpacking ros-rolling-rosbag2-cpp (0.13.0-1focal.20220204.190351) ...
Selecting previously unselected package ros-rolling-rosbag2-compression.
Preparing to unpack .../30-ros-rolling-rosbag2-compression_0.13.0-1focal.20220204.19
1233_amd64.deb ...
Unpacking ros-rolling-rosbag2-compression (0.13.0-1focal.20220204.191233) ...
Selecting previously unselected package ros-rolling-rosbag2-interfaces.
Preparing to unpack .../31-ros-rolling-rosbag2-interfaces_0.13.0-1focal.20220121.214
225_amd64.deb ...
Unpacking ros-rolling-rosbag2-interfaces (0.13.0-1focal.20220121.214225) ...
Selecting previously unselected package ros-rolling-rosbag2-transport.
Preparing to unpack .../32-ros-rolling-rosbag2-transport_0.13.0-1focal.20220204.1923
04_amd64.deb ...
Unpacking ros-rolling-rosbag2-transport (0.13.0-1focal.20220204.192304) ...
Selecting previously unselected package ros-rolling-rosbag2-py.
Preparing to unpack .../33-ros-rolling-rosbag2-py_0.13.0-1focal.20220204.193524_amd6
4.deb ...
Unpacking ros-rolling-rosbag2-py (0.13.0-1focal.20220204.193524) ...
Selecting previously unselected package ros-rolling-ros2bag.
Preparing to unpack .../34-ros-rolling-ros2bag_0.13.0-1focal.20220204.193831_amd64.d
eb ...
Unpacking ros-rolling-ros2bag (0.13.0-1focal.20220204.193831) ...
Selecting previously unselected package ros-rolling-zstd-vendor.
Preparing to unpack .../35-ros-rolling-zstd-vendor_0.13.0-1focal.20220120.181332_amd
64.deb ...
Unpacking ros-rolling-zstd-vendor (0.13.0-1focal.20220120.181332) ...
Selecting previously unselected package ros-rolling-rosbag2-compression-zstd.
Preparing to unpack .../36-ros-rolling-rosbag2-compression-zstd_0.13.0-1focal.202202
04.191850_amd64.deb ...
Unpacking ros-rolling-rosbag2-compression-zstd (0.13.0-1focal.20220204.191850) ...
Selecting previously unselected package ros-rolling-rosbag2.
Preparing to unpack .../37-ros-rolling-rosbag2_0.13.0-1focal.20220204.194704_amd64.d
eb ...
Unpacking ros-rolling-rosbag2 (0.13.0-1focal.20220204.194704) ...
Selecting previously unselected package ros-rolling-rqt-gui.
Preparing to unpack .../38-ros-rolling-rqt-gui_1.1.2-1focal.20220122.073030_amd64.de
b ...
Unpacking ros-rolling-rqt-gui (1.1.2-1focal.20220122.073030) ...
Selecting previously unselected package ros-rolling-rqt-gui-cpp.
Preparing to unpack .../39-ros-rolling-rqt-gui-cpp_1.1.2-1focal.20220122.080244_amd6
4.deb ...
Unpacking ros-rolling-rqt-gui-cpp (1.1.2-1focal.20220122.080244) ...
Selecting previously unselected package ros-rolling-rqt-gui-py.
Preparing to unpack .../40-ros-rolling-rqt-gui-py_1.1.2-1focal.20220122.073306_amd64
.deb ...
Unpacking ros-rolling-rqt-gui-py (1.1.2-1focal.20220122.073306) ...
Selecting previously unselected package ros-rolling-rqt-py-common.
Preparing to unpack .../41-ros-rolling-rqt-py-common_1.1.2-1focal.20220122.073039_am
d64.deb ...
Unpacking ros-rolling-rqt-py-common (1.1.2-1focal.20220122.073039) ...
Selecting previously unselected package ros-rolling-rqt.
Preparing to unpack .../42-ros-rolling-rqt_1.1.2-1focal.20220122.083149_amd64.deb ..
.
Unpacking ros-rolling-rqt (1.1.2-1focal.20220122.083149) ...
Selecting previously unselected package ros-rolling-rqt-console.
Preparing to unpack .../43-ros-rolling-rqt-console_2.0.2-1focal.20220122.073552_amd6
4.deb ...
Unpacking ros-rolling-rqt-console (2.0.2-1focal.20220122.073552) ...
Selecting previously unselected package ros-rolling-rqt-msg.
Preparing to unpack .../44-ros-rolling-rqt-msg_1.0.5-1focal.20220122.073623_amd64.de
b ...
Unpacking ros-rolling-rqt-msg (1.0.5-1focal.20220122.073623) ...
Selecting previously unselected package ros-rolling-rqt-action.
Preparing to unpack .../45-ros-rolling-rqt-action_2.0.1-1focal.20220122.073654_amd64
.deb ...
Unpacking ros-rolling-rqt-action (2.0.1-1focal.20220122.073654) ...
Selecting previously unselected package ros-rolling-rqt-bag.
Preparing to unpack .../46-ros-rolling-rqt-bag_1.1.1-1focal.20220204.193837_amd64.de
b ...
Unpacking ros-rolling-rqt-bag (1.1.1-1focal.20220204.193837) ...
Selecting previously unselected package ros-rolling-rqt-plot.
Preparing to unpack .../47-ros-rolling-rqt-plot_1.1.1-1focal.20220122.073554_amd64.d
eb ...
Unpacking ros-rolling-rqt-plot (1.1.1-1focal.20220122.073554) ...
Selecting previously unselected package ros-rolling-rqt-bag-plugins.
Preparing to unpack .../48-ros-rolling-rqt-bag-plugins_1.1.1-1focal.20220204.194830_
amd64.deb ...
Unpacking ros-rolling-rqt-bag-plugins (1.1.1-1focal.20220204.194830) ...
Selecting previously unselected package ros-rolling-rqt-graph.
Preparing to unpack .../49-ros-rolling-rqt-graph_1.2.1-1focal.20220122.073638_amd64.
deb ...
Unpacking ros-rolling-rqt-graph (1.2.1-1focal.20220122.073638) ...
Selecting previously unselected package ros-rolling-rqt-image-view.
Preparing to unpack .../50-ros-rolling-rqt-image-view_1.1.2-1focal.20220127.231213_a
md64.deb ...
Unpacking ros-rolling-rqt-image-view (1.1.2-1focal.20220127.231213) ...
Selecting previously unselected package ros-rolling-rqt-publisher.
Preparing to unpack .../51-ros-rolling-rqt-publisher_1.1.3-1focal.20220122.073700_am
d64.deb ...
Unpacking ros-rolling-rqt-publisher (1.1.3-1focal.20220122.073700) ...
Selecting previously unselected package ros-rolling-rqt-py-console.
Preparing to unpack .../52-ros-rolling-rqt-py-console_1.0.2-1focal.20220122.073554_a
md64.deb ...
Unpacking ros-rolling-rqt-py-console (1.0.2-1focal.20220122.073554) ...
Selecting previously unselected package ros-rolling-rqt-reconfigure.
Preparing to unpack .../53-ros-rolling-rqt-reconfigure_1.0.8-1focal.20220122.073625_
amd64.deb ...
Unpacking ros-rolling-rqt-reconfigure (1.0.8-1focal.20220122.073625) ...
Selecting previously unselected package ros-rolling-rqt-service-caller.
Preparing to unpack .../54-ros-rolling-rqt-service-caller_1.0.5-1focal.20220122.0736
59_amd64.deb ...
Unpacking ros-rolling-rqt-service-caller (1.0.5-1focal.20220122.073659) ...
Selecting previously unselected package ros-rolling-rqt-shell.
Preparing to unpack .../55-ros-rolling-rqt-shell_1.0.2-1focal.20220122.073705_amd64.
deb ...
Unpacking ros-rolling-rqt-shell (1.0.2-1focal.20220122.073705) ...
Selecting previously unselected package ros-rolling-rqt-srv.
Preparing to unpack .../56-ros-rolling-rqt-srv_1.0.3-1focal.20220122.073654_amd64.de
b ...
Unpacking ros-rolling-rqt-srv (1.0.3-1focal.20220122.073654) ...
Selecting previously unselected package ros-rolling-rqt-top.
Preparing to unpack .../57-ros-rolling-rqt-top_1.0.2-1focal.20220122.073629_amd64.de
b ...
Unpacking ros-rolling-rqt-top (1.0.2-1focal.20220122.073629) ...
Selecting previously unselected package ros-rolling-rqt-topic.
Preparing to unpack .../58-ros-rolling-rqt-topic_1.2.2-1focal.20220122.073711_amd64.
deb ...
Unpacking ros-rolling-rqt-topic (1.2.2-1focal.20220122.073711) ...
Selecting previously unselected package ros-rolling-rqt-common-plugins.
Preparing to unpack .../59-ros-rolling-rqt-common-plugins_1.1.0-1focal.20220204.1949
02_amd64.deb ...
Unpacking ros-rolling-rqt-common-plugins (1.1.0-1focal.20220204.194902) ...
Selecting previously unselected package ros-rolling-rqt-gui-cpp-dbgsym.
Preparing to unpack .../60-ros-rolling-rqt-gui-cpp-dbgsym_1.1.2-1focal.20220122.0802
44_amd64.deb ...
Unpacking ros-rolling-rqt-gui-cpp-dbgsym (1.1.2-1focal.20220122.080244) ...
Selecting previously unselected package ros-rolling-rqt-image-overlay-layer.
Preparing to unpack .../61-ros-rolling-rqt-image-overlay-layer_0.0.2-1focal.20220131
.224047_amd64.deb ...
Unpacking ros-rolling-rqt-image-overlay-layer (0.0.2-1focal.20220131.224047) ...
Selecting previously unselected package ros-rolling-rqt-image-overlay.
Preparing to unpack .../62-ros-rolling-rqt-image-overlay_0.0.2-1focal.20220131.22432
3_amd64.deb ...
Unpacking ros-rolling-rqt-image-overlay (0.0.2-1focal.20220131.224323) ...
Selecting previously unselected package ros-rolling-rqt-image-overlay-dbgsym.
Preparing to unpack .../63-ros-rolling-rqt-image-overlay-dbgsym_0.0.2-1focal.2022013
1.224323_amd64.deb ...
Unpacking ros-rolling-rqt-image-overlay-dbgsym (0.0.2-1focal.20220131.224323) ...
Selecting previously unselected package ros-rolling-rqt-image-view-dbgsym.
Preparing to unpack .../64-ros-rolling-rqt-image-view-dbgsym_1.1.2-1focal.20220127.2
31213_amd64.deb ...
Unpacking ros-rolling-rqt-image-view-dbgsym (1.1.2-1focal.20220127.231213) ...
Selecting previously unselected package ros-rolling-rqt-moveit.
Preparing to unpack .../65-ros-rolling-rqt-moveit_1.0.1-1focal.20220122.073739_amd64
.deb ...
Unpacking ros-rolling-rqt-moveit (1.0.1-1focal.20220122.073739) ...
Selecting previously unselected package ros-rolling-rqt-robot-monitor.
Preparing to unpack .../66-ros-rolling-rqt-robot-monitor_1.0.4-1focal.20220122.07355
7_amd64.deb ...
Unpacking ros-rolling-rqt-robot-monitor (1.0.4-1focal.20220122.073557) ...
Selecting previously unselected package ros-rolling-rqt-robot-dashboard.
Preparing to unpack .../67-ros-rolling-rqt-robot-dashboard_0.6.1-1focal.20220122.073
719_amd64.deb ...
Unpacking ros-rolling-rqt-robot-dashboard (0.6.1-1focal.20220122.073719) ...
Selecting previously unselected package ros-rolling-rqt-robot-steering.
Preparing to unpack .../68-ros-rolling-rqt-robot-steering_1.0.0-2focal.20220122.0736
10_amd64.deb ...
Unpacking ros-rolling-rqt-robot-steering (1.0.0-2focal.20220122.073610) ...
Selecting previously unselected package ros-rolling-rqt-runtime-monitor.
Preparing to unpack .../69-ros-rolling-rqt-runtime-monitor_1.0.0-1focal.20220122.073
621_amd64.deb ...
Unpacking ros-rolling-rqt-runtime-monitor (1.0.0-1focal.20220122.073621) ...
Setting up ros-rolling-yaml-cpp-vendor (8.0.0-1focal.20220204.185241) ...
Setting up python3-rospkg (1.4.0-100) ...
Setting up ros-rolling-lifecycle-msgs (1.1.0-1focal.20220121.213442) ...
Setting up ros-rolling-sensor-msgs (4.0.0-1focal.20220121.220001) ...
Setting up pybind11-dev (2.4.3-2build2) ...
Setting up ros-rolling-console-bridge-vendor (1.3.2-1focal.20220120.195509) ...
Setting up ros-rolling-cv-bridge (3.0.2-2focal.20220127.230816) ...
Setting up ros-rolling-diagnostic-msgs (4.0.0-1focal.20220121.222823) ...
Setting up ros-rolling-tango-icons-vendor (0.1.0-3focal.20220120.195534) ...
Setting up ros-rolling-sqlite3-vendor (0.13.0-1focal.20220120.180903) ...
Setting up ros-rolling-python-qt-binding (1.1.1-1focal.20220120.195235) ...
Setting up ros-rolling-shared-queues-vendor (0.13.0-1focal.20220120.180849) ...
Setting up ros-rolling-rosbag2-interfaces (0.13.0-1focal.20220121.214225) ...
Setting up ros-rolling-zstd-vendor (0.13.0-1focal.20220120.181332) ...
Setting up ros-rolling-keyboard-handler (0.0.3-2focal.20220120.194622) ...
Setting up ros-rolling-tinyxml2-vendor (0.7.4-1focal.20220120.181059) ...
Setting up ros-rolling-rcl-lifecycle (5.0.1-1focal.20220122.071811) ...
Setting up ros-rolling-ros-image-to-qimage (0.0.2-1focal.20220127.231215) ...
Setting up ros-rolling-qt-gui (2.1.1-1focal.20220120.195819) ...
Setting up ros-rolling-class-loader (2.2.0-1focal.20220121.210047) ...
Setting up ros-rolling-pybind11-vendor (2.3.0-1focal.20220120.180711) ...
Setting up ros-rolling-qt-gui-py-common (2.1.1-1focal.20220120.195538) ...
Setting up ros-rolling-qt-dotgraph (2.1.1-1focal.20220120.195537) ...
Setting up ros-rolling-pluginlib (5.1.0-1focal.20220121.210530) ...
Setting up ros-rolling-rclpy (3.2.1-1focal.20220122.072501) ...
Setting up ros-rolling-rqt-image-overlay-layer (0.0.2-1focal.20220131.224047) ...
Setting up ros-rolling-qt-gui-cpp (2.1.1-1focal.20220121.211623) ...
Setting up ros-rolling-rqt-py-common (1.1.2-1focal.20220122.073039) ...
Setting up ros-rolling-ros2cli (0.17.1-1focal.20220126.184012) ...
Setting up ros-rolling-rqt-gui-cpp (1.1.2-1focal.20220122.080244) ...
Setting up ros-rolling-message-filters (4.2.0-1focal.20220122.080945) ...
Setting up ros-rolling-rqt-gui (1.1.2-1focal.20220122.073030) ...
Setting up ros-rolling-image-transport (3.1.2-1focal.20220122.081507) ...
Setting up ros-rolling-rqt-gui-cpp-dbgsym (1.1.2-1focal.20220122.080244) ...
Setting up ros-rolling-rosbag2-storage (0.13.0-1focal.20220204.185423) ...
Setting up ros-rolling-rqt-image-overlay (0.0.2-1focal.20220131.224323) ...
Setting up ros-rolling-rosbag2-storage-default-plugins (0.13.0-1focal.20220204.19012
5) ...
Setting up ros-rolling-rqt-gui-py (1.1.2-1focal.20220122.073306) ...
Setting up ros-rolling-rqt-console (2.0.2-1focal.20220122.073552) ...
Setting up ros-rolling-rqt-service-caller (1.0.5-1focal.20220122.073659) ...
Setting up ros-rolling-rqt-image-view (1.1.2-1focal.20220127.231213) ...
Setting up ros-rolling-rqt-shell (1.0.2-1focal.20220122.073705) ...
Setting up ros-rolling-rqt-robot-monitor (1.0.4-1focal.20220122.073557) ...
Setting up ros-rolling-rqt-image-overlay-dbgsym (0.0.2-1focal.20220131.224323) ...
Setting up ros-rolling-rqt-reconfigure (1.0.8-1focal.20220122.073625) ...
Setting up ros-rolling-rqt-msg (1.0.5-1focal.20220122.073623) ...
Setting up ros-rolling-rosbag2-cpp (0.13.0-1focal.20220204.190351) ...
Setting up ros-rolling-rqt-image-view-dbgsym (1.1.2-1focal.20220127.231213) ...
Setting up ros-rolling-rqt-robot-steering (1.0.0-2focal.20220122.073610) ...
Setting up ros-rolling-rqt-top (1.0.2-1focal.20220122.073629) ...
Setting up ros-rolling-rqt-robot-dashboard (0.6.1-1focal.20220122.073719) ...
Setting up ros-rolling-rqt-topic (1.2.2-1focal.20220122.073711) ...
Setting up ros-rolling-rqt-py-console (1.0.2-1focal.20220122.073554) ...
Setting up ros-rolling-rqt (1.1.2-1focal.20220122.083149) ...
Setting up ros-rolling-rqt-graph (1.2.1-1focal.20220122.073638) ...
Setting up ros-rolling-rqt-publisher (1.1.3-1focal.20220122.073700) ...
Setting up ros-rolling-rqt-runtime-monitor (1.0.0-1focal.20220122.073621) ...
Setting up ros-rolling-rqt-plot (1.1.1-1focal.20220122.073554) ...
Setting up ros-rolling-rosbag2-compression (0.13.0-1focal.20220204.191233) ...
Setting up ros-rolling-rqt-srv (1.0.3-1focal.20220122.073654) ...
Setting up ros-rolling-rqt-action (2.0.1-1focal.20220122.073654) ...
Setting up ros-rolling-rqt-moveit (1.0.1-1focal.20220122.073739) ...
Setting up ros-rolling-rosbag2-compression-zstd (0.13.0-1focal.20220204.191850) ...
Setting up ros-rolling-rosbag2-transport (0.13.0-1focal.20220204.192304) ...
Setting up ros-rolling-rosbag2-py (0.13.0-1focal.20220204.193524) ...
Setting up ros-rolling-rqt-bag (1.1.1-1focal.20220204.193837) ...
Setting up ros-rolling-ros2bag (0.13.0-1focal.20220204.193831) ...
Setting up ros-rolling-rosbag2 (0.13.0-1focal.20220204.194704) ...
Setting up ros-rolling-rqt-bag-plugins (1.1.1-1focal.20220204.194830) ...
Setting up ros-rolling-rqt-common-plugins (1.1.0-1focal.20220204.194902) ...
Processing triggers for libc-bin (2.31-0ubuntu9.9) ...
muslimjon@ubuntu:~$ rqt 
```
![Screenshot from 2022-10-18 18-58-02](https://user-images.githubusercontent.com/114977921/196579387-59391932-1b8b-4c6c-bfcb-f0a72ed439e8.png)


![Screenshot from 2022-10-18 22-17-07](https://user-images.githubusercontent.com/114977921/196603500-7b3de326-7b26-42e7-b799-97bfc3c6aff1.png)
## ROS2 Colcon
```
muslimjon@ubuntu:~$ mkdir -p ~/ros2_ws/src
muslimjon@ubuntu:~$ cd ~/ros2_ws
muslimjon@ubuntu:~/ros2_ws$ git clone https://github.com/ros2/examples src/examples -b foxy
fatal: destination path 'src/examples' already exists and is not an empty directory.
```
```
muslimjon@ubuntu:~/ros2_ws$ colcon build --symlink-install
[0.500s] WARNING:colcon.colcon_core.package_selection:Some selected packages are already built in one or more underlay workspaces:
	'examples_rclcpp_minimal_timer' is in: /opt/ros/foxy
	'examples_rclcpp_minimal_action_client' is in: /opt/ros/foxy
	'examples_rclcpp_minimal_subscriber' is in: /opt/ros/foxy
	'examples_rclcpp_minimal_client' is in: /opt/ros/foxy
	'examples_rclcpp_minimal_composition' is in: /opt/ros/foxy
	'examples_rclpy_minimal_action_client' is in: /opt/ros/foxy
	'examples_rclcpp_minimal_publisher' is in: /opt/ros/foxy
	'examples_rclpy_minimal_subscriber' is in: /opt/ros/foxy
	'examples_rclcpp_minimal_service' is in: /opt/ros/foxy
	'examples_rclpy_executors' is in: /opt/ros/foxy
	'examples_rclpy_minimal_service' is in: /opt/ros/foxy
	'turtlesim' is in: /opt/ros/foxy
	'examples_rclcpp_minimal_action_server' is in: /opt/ros/foxy
	'examples_rclpy_minimal_publisher' is in: /opt/ros/foxy
	'examples_rclpy_minimal_client' is in: /opt/ros/foxy
	'examples_rclcpp_multithreaded_executor' is in: /opt/ros/foxy
	'examples_rclpy_minimal_action_server' is in: /opt/ros/foxy
If a package in a merged underlay workspace is overridden and it installs headers, then all packages in the overlay must sort their include directories by workspace order. Failure to do so may result in build failures or undefined behavior at run time.
If the overridden package is used by another package in any underlay, then the overriding package in the overlay must be API and ABI compatible or undefined behavior at run time may occur.

If you understand the risks and want to override a package anyways, add the following to the command line:
	--allow-overriding examples_rclcpp_minimal_action_client examples_rclcpp_minimal_action_server examples_rclcpp_minimal_client examples_rclcpp_minimal_composition examples_rclcpp_minimal_publisher examples_rclcpp_minimal_service examples_rclcpp_minimal_subscriber examples_rclcpp_minimal_timer examples_rclcpp_multithreaded_executor examples_rclpy_executors examples_rclpy_minimal_action_client examples_rclpy_minimal_action_server examples_rclpy_minimal_client examples_rclpy_minimal_publisher examples_rclpy_minimal_service examples_rclpy_minimal_subscriber turtlesim

This may be promoted to an error in a future release of colcon-override-check.
Starting >>> examples_rclcpp_minimal_action_client
Starting >>> examples_rclcpp_minimal_action_server
Finished <<< examples_rclcpp_minimal_action_server [0.44s]
Starting >>> examples_rclcpp_minimal_client
Finished <<< examples_rclcpp_minimal_action_client [0.59s]
Starting >>> examples_rclcpp_minimal_composition
Finished <<< examples_rclcpp_minimal_client [0.42s]
Starting >>> examples_rclcpp_minimal_publisher
Finished <<< examples_rclcpp_minimal_composition [0.55s]
Starting >>> examples_rclcpp_minimal_service
Finished <<< examples_rclcpp_minimal_publisher [0.42s]
Starting >>> examples_rclcpp_minimal_subscriber                           
Finished <<< examples_rclcpp_minimal_service [0.38s]
Starting >>> examples_rclcpp_minimal_timer
Finished <<< examples_rclcpp_minimal_subscriber [0.45s]
Starting >>> examples_rclcpp_multithreaded_executor
Finished <<< examples_rclcpp_minimal_timer [0.39s]
Starting >>> examples_rclpy_executors
Finished <<< examples_rclcpp_multithreaded_executor [0.61s]
Starting >>> examples_rclpy_minimal_action_client
Finished <<< examples_rclpy_executors [1.38s]                           
Starting >>> examples_rclpy_minimal_action_server
Finished <<< examples_rclpy_minimal_action_client [1.32s]
Starting >>> examples_rclpy_minimal_client
Finished <<< examples_rclpy_minimal_action_server [1.35s]
Starting >>> examples_rclpy_minimal_publisher
Finished <<< examples_rclpy_minimal_client [1.36s]                            
Starting >>> examples_rclpy_minimal_service
Finished <<< examples_rclpy_minimal_publisher [1.33s]
Starting >>> examples_rclpy_minimal_subscriber
Finished <<< examples_rclpy_minimal_service [1.37s]                            
Starting >>> musimjon
Finished <<< examples_rclpy_minimal_subscriber [1.95s]
Starting >>> turtlesim
Finished <<< musimjon [2.13s]                                                 
--- stderr: turtlesim                            
CMake Error at CMakeLists.txt:47 (rosidl_get_typesupport_target):
  Unknown CMake command "rosidl_get_typesupport_target".


---
Failed   <<< turtlesim [3.07s, exited with code 1]

Summary: 17 packages finished [11.4s]
  1 package failed: turtlesim
  1 package had stderr output: turtlesim
  ```
  ```
  muslimjon@ubuntu:~/ros2_ws$ colcon test
Starting >>> examples_rclcpp_minimal_action_client
Starting >>> examples_rclcpp_minimal_action_server
Finished <<< examples_rclcpp_minimal_action_server [2.77s]
Starting >>> examples_rclcpp_minimal_client
Finished <<< examples_rclcpp_minimal_action_client [2.82s]
Starting >>> examples_rclcpp_minimal_composition
Finished <<< examples_rclcpp_minimal_client [2.81s]                           
Starting >>> examples_rclcpp_minimal_publisher
Finished <<< examples_rclcpp_minimal_composition [2.90s]
Starting >>> examples_rclcpp_minimal_service
Finished <<< examples_rclcpp_minimal_service [3.76s]
Starting >>> examples_rclcpp_minimal_subscriber                  
Finished <<< examples_rclcpp_minimal_publisher [3.92s]
Starting >>> examples_rclcpp_minimal_timer
Finished <<< examples_rclcpp_minimal_subscriber [2.79s]
Starting >>> examples_rclcpp_multithreaded_executor
Finished <<< examples_rclcpp_minimal_timer [2.79s]                            
Starting >>> examples_rclpy_executors
--- stderr: examples_rclpy_executors   

=============================== warnings summary ===============================
/usr/lib/python3/dist-packages/pydocstyle/config.py:6
  Warning: Using or importing the ABCs from 'collections' instead of from 'collections.abc' is deprecated since Python 3.3, and in 3.10 it will stop working

-- Docs: https://docs.pytest.org/en/latest/warnings.html
---
Finished <<< examples_rclpy_executors [1.57s]
Starting >>> examples_rclpy_minimal_action_client
Finished <<< examples_rclcpp_multithreaded_executor [2.64s]
Starting >>> examples_rclpy_minimal_action_server
--- stderr: examples_rclpy_minimal_action_client

=============================== warnings summary ===============================
/usr/lib/python3/dist-packages/pydocstyle/config.py:6
  Warning: Using or importing the ABCs from 'collections' instead of from 'collections.abc' is deprecated since Python 3.3, and in 3.10 it will stop working

-- Docs: https://docs.pytest.org/en/latest/warnings.html
---
Finished <<< examples_rclpy_minimal_action_client [1.36s]
Starting >>> examples_rclpy_minimal_client
--- stderr: examples_rclpy_minimal_action_server

=============================== warnings summary ===============================
/usr/lib/python3/dist-packages/pydocstyle/config.py:6
  Warning: Using or importing the ABCs from 'collections' instead of from 'collections.abc' is deprecated since Python 3.3, and in 3.10 it will stop working

-- Docs: https://docs.pytest.org/en/latest/warnings.html
---
Finished <<< examples_rclpy_minimal_action_server [1.37s]
Starting >>> examples_rclpy_minimal_publisher
--- stderr: examples_rclpy_minimal_client                                      

=============================== warnings summary ===============================
/usr/lib/python3/dist-packages/pydocstyle/config.py:6
  Warning: Using or importing the ABCs from 'collections' instead of from 'collections.abc' is deprecated since Python 3.3, and in 3.10 it will stop working

-- Docs: https://docs.pytest.org/en/latest/warnings.html
---
Finished <<< examples_rclpy_minimal_client [1.36s]
Starting >>> examples_rclpy_minimal_service
--- stderr: examples_rclpy_minimal_publisher

=============================== warnings summary ===============================
/usr/lib/python3/dist-packages/pydocstyle/config.py:6
  Warning: Using or importing the ABCs from 'collections' instead of from 'collections.abc' is deprecated since Python 3.3, and in 3.10 it will stop working

-- Docs: https://docs.pytest.org/en/latest/warnings.html
---
Finished <<< examples_rclpy_minimal_publisher [1.28s]
Starting >>> examples_rclpy_minimal_subscriber
--- stderr: examples_rclpy_minimal_service

=============================== warnings summary ===============================
/usr/lib/python3/dist-packages/pydocstyle/config.py:6
  Warning: Using or importing the ABCs from 'collections' instead of from 'collections.abc' is deprecated since Python 3.3, and in 3.10 it will stop working

-- Docs: https://docs.pytest.org/en/latest/warnings.html
---
Finished <<< examples_rclpy_minimal_service [1.28s]
Starting >>> musimjon
--- stderr: examples_rclpy_minimal_subscriber

=============================== warnings summary ===============================
/usr/lib/python3/dist-packages/pydocstyle/config.py:6
  Warning: Using or importing the ABCs from 'collections' instead of from 'collections.abc' is deprecated since Python 3.3, and in 3.10 it will stop working

-- Docs: https://docs.pytest.org/en/latest/warnings.html
---
Finished <<< examples_rclpy_minimal_subscriber [1.25s]
Starting >>> turtlesim
Finished <<< turtlesim [0.03s]
Finished <<< musimjon [1.47s]             

Summary: 18 packages finished [19.7s]
  7 packages had stderr output: examples_rclpy_executors examples_rclpy_minimal_action_client examples_rclpy_minimal_action_server examples_rclpy_minimal_client examples_rclpy_minimal_publisher examples_rclpy_minimal_service examples_rclpy_minimal_subscriber
muslimjon@ubuntu:~/ros2_ws$ 
```
  
