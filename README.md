# Task-2-ROS-noetic

install ROS Neotic on Ubuntu

1.  download VirtualBox.
2.  download [Ubuntu 20.04.4](https://releases.ubuntu.com/20.04.4/?_ga=2.254970826.372918294.1658034976-1795708661.1658034976).
3. create the virttual machine.

## install ROS Noetic

**Setup your sources.list**

Setup your computer to accept software from packages.ros.org.

``` sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'```

**Set up your keys**

```
sudo apt install curl # if you haven't already installed curl
curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -
```

**Installation**

First, make sure your Debian package index is up-to-date

`sudo apt update`

**Desktop-Full Install: (Recommended) :**: Everything in Desktop plus 2D/3D simulators and 2D/3D perception packages

**sudo apt install ros-noetic-desktop-full**

`sudo apt install ros-noetic-desktop-full`

**Environment setup**
```
echo "source /opt/ros/noetic/setup.bash" >> ~/.bashrc
source ~/.bashrc
 ```
 **Dependencies for building packages**

 `sudo apt install python3-rosdep python3-rosinstall python3-rosinstall
-generator python3-wstool build-essential`

**Initialize rosdep**
```
 sudo apt install python3-rosdep
 sudo rosdep init
 rosdep update
```

**start the ROS**

`roscore`
