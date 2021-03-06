.. _i_gms2_class_binary:

Class: Binary
=============

Binary file instances are essentially an in-memory reference to the contents of an Open Day Dialogue binary file. They can be loaded and unloaded as the game wishes.

Binary file instances be created with two functions:

.. toctree::
   :maxdepth: 1
   
   func_odd_load_binary
   func_odd_load_binary_from_buffer

Binary file instances can be unloaded/destroyed with this function:

.. toctree::
   :maxdepth: 1
   
   func_odd_unload_binary
   
.. attention:: It is recommended that you unload a binary file instance once it is no longer in use.