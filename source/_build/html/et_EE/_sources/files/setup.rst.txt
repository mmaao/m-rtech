
#####
Setup
#####

.. toctree::
   :maxdepth: 2


Installing Ubuntu
-----------------

Download and install Ubuntu Linux on your PC from the following link: `Ubuntu 18.04.4 LTS (Bionic Beaver) <http://releases.ubuntu.com/18.04.4/?_ga=2.170843936.1678816316.1594710587-1973467440.1591964081>`__.

The guide to install Ubuntu on your PC can be found `here <https://ubuntu.com/tutorials/install-ubuntu-desktop#1-overview>`__.

Installing ROS
--------------

Install Ros Melodic according to the following link: `Ros Melodic <http://wiki.ros.org/melodic/Installation/Ubuntu>`__.

.. _connecting-remotely:

Connecting remotely
--------------------

1. Open a new terminal window
2. connect the user PC to ROBOTONT's network or make sure that the user PC and ROBOTONT's on-board computer are connected to the same wifi router 

  .. image:: /files/pictures/wifi_screen.png
    :width: 400

3. Establish an ssh connection (change the X with the ID written on the robot)

   .. code-block:: bash
      
      ssh kasutaja@clearbot-X

  or 

  .. code-block:: bash
      
      ssh kasutaja@ip_of_the_robot

  .. image:: /files/pictures/ssh_nt.png
    :width: 400

4. Enter the password: t0ndik00bas

5. When logged in successfully, you can see that the terminal prompt has changed to kasutaja@clearbot-X. This will be an important reference when trying to figure out which terminal is connected to where.

  .. image:: /files/pictures/ssh_nt2.png
    :width: 400

6. After logging into the robot, the ROS environment should be automatically sourced for you. You can quickly display the last lines of the file with tail ~/.bashrc command to examine which workspaces are sourced.