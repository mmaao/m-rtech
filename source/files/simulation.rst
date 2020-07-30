##########
Simulation
##########

Launching the Simulation
------------------------

#. To launch the simulator and drive around: 

   .. code-block:: bash
      
      roslaunch robotont_gazebo gazebo_teleop_keyboard.launch

Mapping
-------

gmapping
********

#. Launch the simulator

   .. code-block:: bash
      
      roslaunch robotont_gazebo gazebo_teleop_keyboard.launch

#. Launch the gmapping software

   .. code-block:: bash
      
      roslaunch robotont_gazebo gazebo_gmapping.launch

#. Drive around using the keyboard and map the world

Google Cartographer
*******************
#. Launch the simulator

   .. code-block:: bash
      
      roslaunch robotont_gazebo gazebo_teleop_keyboard.launch

#. Launch the gmapping software

   .. code-block:: bash
      
      roslaunch robotont_gazebo 2d_nav_carto_gazebo.launch
    
#. Drive around using the keyboard and map the world
