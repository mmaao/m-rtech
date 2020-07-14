
###############
Installing ROS
###############


#. Set up sources.list

   .. code-block:: bash
   
      sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'

#. Set up ROS keys

   .. code-block:: bash
   
      sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654

#. Install ROS Melodic

   .. code-block:: bash

      sudo apt update
      sudo apt install ros-melodic-desktop-full

#. Environment setup

   .. code-block:: bash

        echo "source /opt/ros/melodic/setup.bash" >> ~/.bashrc
        source ~/.bashrc


#. Initialize rosdep

   .. code-block:: bash

        sudo apt install python-rosdep
        sudo rosdep init
        rosdep update