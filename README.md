# ros-installation
### Step 1: Setup your sources.list
```
sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
```
### Step 2: Set up your keys
```
sudo apt install curl # if you haven't already installed curl
curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -
```


### step 3: Installation
first updating 
``` 
sudo apt update
```

###step 4: Installation Desktop-Full :
```
sudo apt install ros-noetic-desktop-full
```

###step 5: Environment setup

```
source /opt/ros/noetic/setup.bash
```
###step 6: Bash

```
echo "source /opt/ros/noetic/setup.bash" >> ~/.bashrc
source ~/.bashrc
```

###step 7:  Dependencies for building packages
```
sudo apt install python3-rosdep python3-rosinstall python3-rosinstall-generator python3-wstool build-essential
```

###step 8:  Initialize rosdep

```
sudo apt install python3-rosdep
```
###step 9:  With the following, you can initialize rosdep.


```
sudo rosdep init
rosdep update
```



###step 10:roscore

```
roscore
```


