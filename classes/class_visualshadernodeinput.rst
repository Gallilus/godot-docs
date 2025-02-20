:github_url: hide

.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the VisualShaderNodeInput.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_VisualShaderNodeInput:

VisualShaderNodeInput
=====================

**Inherits:** :ref:`VisualShaderNode<class_VisualShaderNode>` **<** :ref:`Resource<class_Resource>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

Represents the input shader parameter within the visual shader graph.

Description
-----------

Gives access to input variables (built-ins) available for the shader. See the shading reference for the list of available built-ins for each shader type (check ``Tutorials`` section for link).

Tutorials
---------

- :doc:`../tutorials/shaders/shader_reference/index`

Properties
----------

+-----------------------------+--------------------------------------------------------------------+--------------+
| :ref:`String<class_String>` | :ref:`input_name<class_VisualShaderNodeInput_property_input_name>` | ``"[None]"`` |
+-----------------------------+--------------------------------------------------------------------+--------------+

Methods
-------

+-----------------------------+--------------------------------------------------------------------------------------------------------+
| :ref:`String<class_String>` | :ref:`get_input_real_name<class_VisualShaderNodeInput_method_get_input_real_name>` **(** **)** |const| |
+-----------------------------+--------------------------------------------------------------------------------------------------------+

Signals
-------

.. _class_VisualShaderNodeInput_signal_input_type_changed:

- **input_type_changed** **(** **)**

Emitted when input is changed via :ref:`input_name<class_VisualShaderNodeInput_property_input_name>`.

Property Descriptions
---------------------

.. _class_VisualShaderNodeInput_property_input_name:

- :ref:`String<class_String>` **input_name**

+-----------+-----------------------+
| *Default* | ``"[None]"``          |
+-----------+-----------------------+
| *Setter*  | set_input_name(value) |
+-----------+-----------------------+
| *Getter*  | get_input_name()      |
+-----------+-----------------------+

One of the several input constants in lower-case style like: "vertex"(``VERTEX``) or "point_size"(``POINT_SIZE``).

Method Descriptions
-------------------

.. _class_VisualShaderNodeInput_method_get_input_real_name:

- :ref:`String<class_String>` **get_input_real_name** **(** **)** |const|

Returns a translated name of the current constant in the Godot Shader Language. E.g. ``"ALBEDO"`` if the :ref:`input_name<class_VisualShaderNodeInput_property_input_name>` equal to ``"albedo"``.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
