.. _i_gms2_func_odd_value_convert:

odd_value_convert
=================

Syntax
------

.. code-block:: c

    odd_value_convert(value, type)

Parameters
----------
+------+-----------------------------------------+
|Name  |Description                              |
+======+=========================================+
|value |The :ref:`Value<i_gms2_class_value>`     |
|      |to convert.                              |
+------+-----------------------------------------+
|type  |The :ref:`odd_type<i_gms2_enum_odd_type>`|
|      |to convert to.                           |
+------+-----------------------------------------+

Returns
-------

A new :ref:`Value<i_gms2_class_value>` with the given type.

Description
-----------

This function will convert any Value into another type, converting the GameMaker value it holds as well.

Example
-------

.. code-block:: js

    var value = odd_create_value(odd_type_int32, 21);

    var newValue = odd_value_convert(value, odd_type_string);

    show_debug_message(odd_value_val(newValue));

    // ...

This would print "21" to the console, without using string() because the value was converted to a string as well.