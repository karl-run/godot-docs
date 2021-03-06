.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the GraphNode.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_GraphNode:

GraphNode
=========

**Inherits:** :ref:`Container<class_container>` **<** :ref:`Control<class_control>` **<** :ref:`CanvasItem<class_canvasitem>` **<** :ref:`Node<class_node>` **<** :ref:`Object<class_object>`

**Category:** Core

Brief Description
-----------------

A GraphNode is a container with several input and output slots allowing connections between GraphNodes. Slots can have different, incompatible types.

Member Functions
----------------

+--------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                           | :ref:`clear_all_slots<class_GraphNode_clear_all_slots>` **(** **)**                                                                                                                                                                                                                                                                                                                                         |
+--------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                           | :ref:`clear_slot<class_GraphNode_clear_slot>` **(** :ref:`int<class_int>` idx **)**                                                                                                                                                                                                                                                                                                                         |
+--------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Color<class_color>`      | :ref:`get_connection_input_color<class_GraphNode_get_connection_input_color>` **(** :ref:`int<class_int>` idx **)**                                                                                                                                                                                                                                                                                         |
+--------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`          | :ref:`get_connection_input_count<class_GraphNode_get_connection_input_count>` **(** **)**                                                                                                                                                                                                                                                                                                                   |
+--------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector2<class_vector2>`  | :ref:`get_connection_input_position<class_GraphNode_get_connection_input_position>` **(** :ref:`int<class_int>` idx **)**                                                                                                                                                                                                                                                                                   |
+--------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`          | :ref:`get_connection_input_type<class_GraphNode_get_connection_input_type>` **(** :ref:`int<class_int>` idx **)**                                                                                                                                                                                                                                                                                           |
+--------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Color<class_color>`      | :ref:`get_connection_output_color<class_GraphNode_get_connection_output_color>` **(** :ref:`int<class_int>` idx **)**                                                                                                                                                                                                                                                                                       |
+--------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`          | :ref:`get_connection_output_count<class_GraphNode_get_connection_output_count>` **(** **)**                                                                                                                                                                                                                                                                                                                 |
+--------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector2<class_vector2>`  | :ref:`get_connection_output_position<class_GraphNode_get_connection_output_position>` **(** :ref:`int<class_int>` idx **)**                                                                                                                                                                                                                                                                                 |
+--------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`          | :ref:`get_connection_output_type<class_GraphNode_get_connection_output_type>` **(** :ref:`int<class_int>` idx **)**                                                                                                                                                                                                                                                                                         |
+--------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Color<class_color>`      | :ref:`get_slot_color_left<class_GraphNode_get_slot_color_left>` **(** :ref:`int<class_int>` idx **)** const                                                                                                                                                                                                                                                                                                 |
+--------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Color<class_color>`      | :ref:`get_slot_color_right<class_GraphNode_get_slot_color_right>` **(** :ref:`int<class_int>` idx **)** const                                                                                                                                                                                                                                                                                               |
+--------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`          | :ref:`get_slot_type_left<class_GraphNode_get_slot_type_left>` **(** :ref:`int<class_int>` idx **)** const                                                                                                                                                                                                                                                                                                   |
+--------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`          | :ref:`get_slot_type_right<class_GraphNode_get_slot_type_right>` **(** :ref:`int<class_int>` idx **)** const                                                                                                                                                                                                                                                                                                 |
+--------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`        | :ref:`is_slot_enabled_left<class_GraphNode_is_slot_enabled_left>` **(** :ref:`int<class_int>` idx **)** const                                                                                                                                                                                                                                                                                               |
+--------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`        | :ref:`is_slot_enabled_right<class_GraphNode_is_slot_enabled_right>` **(** :ref:`int<class_int>` idx **)** const                                                                                                                                                                                                                                                                                             |
+--------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                           | :ref:`set_slot<class_GraphNode_set_slot>` **(** :ref:`int<class_int>` idx, :ref:`bool<class_bool>` enable_left, :ref:`int<class_int>` type_left, :ref:`Color<class_color>` color_left, :ref:`bool<class_bool>` enable_right, :ref:`int<class_int>` type_right, :ref:`Color<class_color>` color_right, :ref:`Texture<class_texture>` custom_left=null, :ref:`Texture<class_texture>` custom_right=null **)** |
+--------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Signals
-------

.. _class_GraphNode_close_request:

- **close_request** **(** **)**

Signal sent on closing the GraphNode.

.. _class_GraphNode_dragged:

- **dragged** **(** :ref:`Vector2<class_vector2>` from, :ref:`Vector2<class_vector2>` to **)**

Signal sent when the GraphNode is dragged.

.. _class_GraphNode_offset_changed:

- **offset_changed** **(** **)**

Signal sent when the GraphNode is moved.

.. _class_GraphNode_raise_request:

- **raise_request** **(** **)**

Signal sent when the GraphNode is requested to be displayed over other ones. Happens on focusing (clicking into) the GraphNode.

.. _class_GraphNode_resize_request:

- **resize_request** **(** :ref:`Vector2<class_vector2>` new_minsize **)**


Member Variables
----------------

  .. _class_GraphNode_comment:

- :ref:`bool<class_bool>` **comment**

  .. _class_GraphNode_offset:

- :ref:`Vector2<class_vector2>` **offset** - The offset of the GraphNode, relative to the scroll offset of the :ref:`GraphEdit<class_graphedit>`. Note that you cannot use position directly, as :ref:`GraphEdit<class_graphedit>` is a :ref:`Container<class_container>`.

  .. _class_GraphNode_overlay:

- :ref:`Overlay<enum_graphnode_overlay>` **overlay**

  .. _class_GraphNode_resizable:

- :ref:`bool<class_bool>` **resizable**

  .. _class_GraphNode_selected:

- :ref:`bool<class_bool>` **selected**

  .. _class_GraphNode_show_close:

- :ref:`bool<class_bool>` **show_close**

  .. _class_GraphNode_title:

- :ref:`String<class_string>` **title**


Enums
-----

  .. _enum_GraphNode_Overlay:

enum **Overlay**

- **OVERLAY_DISABLED** = **0**
- **OVERLAY_BREAKPOINT** = **1**
- **OVERLAY_POSITION** = **2**


Description
-----------

A GraphNode is a container defined by a title. It can have 1 or more input and output slots, which can be enabled (shown) or disabled (not shown) and have different (incompatible) types. Colors can also be assigned to slots. A tuple of input and output slots is defined for each GUI element included in the GraphNode. Input and output connections are left and right slots, but only enabled slots are counted as connections.

Member Function Description
---------------------------

.. _class_GraphNode_clear_all_slots:

- void **clear_all_slots** **(** **)**

Disable all input and output slots of the GraphNode.

.. _class_GraphNode_clear_slot:

- void **clear_slot** **(** :ref:`int<class_int>` idx **)**

Disable input and output slot whose index is 'idx'.

.. _class_GraphNode_get_connection_input_color:

- :ref:`Color<class_color>` **get_connection_input_color** **(** :ref:`int<class_int>` idx **)**

Return the color of the input connection 'idx'.

.. _class_GraphNode_get_connection_input_count:

- :ref:`int<class_int>` **get_connection_input_count** **(** **)**

Return the number of enabled input slots (connections) to the GraphNode.

.. _class_GraphNode_get_connection_input_position:

- :ref:`Vector2<class_vector2>` **get_connection_input_position** **(** :ref:`int<class_int>` idx **)**

Return the position of the input connection 'idx'.

.. _class_GraphNode_get_connection_input_type:

- :ref:`int<class_int>` **get_connection_input_type** **(** :ref:`int<class_int>` idx **)**

Return the type of the input connection 'idx'.

.. _class_GraphNode_get_connection_output_color:

- :ref:`Color<class_color>` **get_connection_output_color** **(** :ref:`int<class_int>` idx **)**

Return the color of the output connection 'idx'.

.. _class_GraphNode_get_connection_output_count:

- :ref:`int<class_int>` **get_connection_output_count** **(** **)**

Return the number of enabled output slots (connections) of the GraphNode.

.. _class_GraphNode_get_connection_output_position:

- :ref:`Vector2<class_vector2>` **get_connection_output_position** **(** :ref:`int<class_int>` idx **)**

Return the position of the output connection 'idx'.

.. _class_GraphNode_get_connection_output_type:

- :ref:`int<class_int>` **get_connection_output_type** **(** :ref:`int<class_int>` idx **)**

Return the type of the output connection 'idx'.

.. _class_GraphNode_get_slot_color_left:

- :ref:`Color<class_color>` **get_slot_color_left** **(** :ref:`int<class_int>` idx **)** const

Return the color set to 'idx' left (input) slot.

.. _class_GraphNode_get_slot_color_right:

- :ref:`Color<class_color>` **get_slot_color_right** **(** :ref:`int<class_int>` idx **)** const

Return the color set to 'idx' right (output) slot.

.. _class_GraphNode_get_slot_type_left:

- :ref:`int<class_int>` **get_slot_type_left** **(** :ref:`int<class_int>` idx **)** const

Return the (integer) type of left (input) 'idx' slot.

.. _class_GraphNode_get_slot_type_right:

- :ref:`int<class_int>` **get_slot_type_right** **(** :ref:`int<class_int>` idx **)** const

Return the (integer) type of right (output) 'idx' slot.

.. _class_GraphNode_is_slot_enabled_left:

- :ref:`bool<class_bool>` **is_slot_enabled_left** **(** :ref:`int<class_int>` idx **)** const

Return true if left (input) slot 'idx' is enabled. False otherwise.

.. _class_GraphNode_is_slot_enabled_right:

- :ref:`bool<class_bool>` **is_slot_enabled_right** **(** :ref:`int<class_int>` idx **)** const

Return true if right (output) slot 'idx' is enabled. False otherwise.

.. _class_GraphNode_set_slot:

- void **set_slot** **(** :ref:`int<class_int>` idx, :ref:`bool<class_bool>` enable_left, :ref:`int<class_int>` type_left, :ref:`Color<class_color>` color_left, :ref:`bool<class_bool>` enable_right, :ref:`int<class_int>` type_right, :ref:`Color<class_color>` color_right, :ref:`Texture<class_texture>` custom_left=null, :ref:`Texture<class_texture>` custom_right=null **)**


