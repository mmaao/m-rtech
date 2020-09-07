################
Simulated robot
################


#. To launch the simulator and drive around: 

   .. code-block:: bash
      
      roslaunch robotont_gazebo gazebo_teleop_keyboard.launch

Maps
----

#. maze.world

   .. image:: /files/pictures/maze.png
      :width: 400

   To run

   .. code-block:: bash
      
      roslaunch robotont_gazebo gazebo_teleop_keyboard.launch world:=$(rospack find robotont_gazebo)/worlds/maze.world

#. bangbang.world

   .. image:: /files/pictures/bangbang.png
      :width: 400

   To run 

   .. code-block:: bash
      
      roslaunch robotont_gazebo gazebo_teleop_keyboard.launch world:=$(rospack find robotont_gazebo)/worlds/bangbang.world x_pos:=0

#. between.world

   .. image:: /files/pictures/between.png
      :width: 400

   To run

   .. code-block:: bash
      
      roslaunch robotont_gazebo gazebo_teleop_keyboard.launch world:=$(rospack find robotont_gazebo)/worlds/between.world x_pos:=0


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
