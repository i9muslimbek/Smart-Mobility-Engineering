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

