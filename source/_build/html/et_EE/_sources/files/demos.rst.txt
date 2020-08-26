
#####
Demos
#####

Before starting establish an ssh connection between the robot and the user PC as shown here: :ref:`connecting-remotely`.

The following packages are needed to run the demos:

#. For 2D mapping:

   .. code-block:: bash
      
      sudo apt update
      sudo apt install ros-melodic-depthimage-to-laserscan
      sudo apt install ros-melodic-cartographer-ros
      sudo apt install ros-melodic-move-base

#. For 3D mapping:

   .. code-block:: bash
      
      sudo apt install ros-melodic-rtabmap-ros

#. For AR tracking:

   .. code-block:: bash
      
      sudo apt install ros-melodic-ar-track-alvar
 


2D mapping
----------

#. **On ROBOTONT on-board computer** launch 2d_nav_carto.launch

   .. code-block:: bash
      
      roslaunch robotont_demos 2d_nav_carto.launch

#. **On the user PC** launch display_2d_mapping.launch to visualize the result

   .. code-block:: bash
      
      roslaunch robotont_demos display_2d_mapping.launch

#. To move the robot open another terminal window **on the user PC** and run teleop twist keyboard

   .. code-block:: bash
      
      rosrun teleop_twist_keyboard teleop_twist_keyboard.py __ns:=/robotont

   .. hint:: Notice that the teleop node only receives keypresses only when the terminal window is active.

3D mapping
----------

#. **On ROBOTONT on-board computer** launch 3d_mapping.launch

   .. code-block:: bash
      
      roslaunch robotont_demos 3d_mapping.launch

#. **On the user PC** launch display_3d_mapping.launch to visualize the result

   .. code-block:: bash
      
      roslaunch robotont_demos display_3d_mapping.launch

#. To move the robot open another terminal window **on the user PC** and run teleop twist keyboard

   .. code-block:: bash
      
      rosrun teleop_twist_keyboard teleop_twist_keyboard.py __ns:=/robotont

   .. hint:: Notice that the teleop node only receives keypresses only when the terminal window is active.

  .. image:: /files/pictures/3dmap.png
    :width: 400

AR tracking
-----------
#. **On ROBOTONT on-board computer** launch ar_follow_the_leader.launch

   .. code-block:: bash
      
      roslaunch roslaunch robotont_demos ar_follow_the_leader.launch

#. **On the user PC** launch display_ar_marker.launch to visualize the result

   .. code-block:: bash
      
      roslaunch robotont_demos display_ar_marker.launch marker_id:=tag_nr

#. To move the robot open another terminal window **on the user PC** and run teleop twist keyboard

   .. code-block:: bash
      
      rosrun teleop_twist_keyboard teleop_twist_keyboard.py __ns:=/robotont
    
    
   .. hint:: Notice that the teleop node only receives keypresses only when the terminal window is active.
