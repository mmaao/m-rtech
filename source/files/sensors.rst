#######
Sensors
#######

ROBOTONT uses a Realsense D435 3D camera, which provides a regular camera feed and a depth sensor. 

The camera feed is launched automatically when the robot is turned on.

Displaying the camera feed
--------------------------

#. Establish an ssh connection between the robot and the user PC as shown here: :ref:`connecting-remotely`

#. **On the user PC** display the feed on RViz


   .. code-block:: bash
      
      roslaunch robotont_demos display_camera.launch


Getting distances from objects
------------------------------

#. Run laserscan_to_distance node

   .. code-block:: bash
      
      roslaunch robotont_laserscan_to_distance distance_from_depth_image.launch

#. To display the messages published to scan_to_distance

   .. code-block:: bash
      
      rostopic echo /scan_to_distance