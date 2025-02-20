:github_url: hide

.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the VisualShaderNodeVectorDerivativeFunc.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_VisualShaderNodeVectorDerivativeFunc:

VisualShaderNodeVectorDerivativeFunc
====================================

**Inherits:** :ref:`VisualShaderNode<class_VisualShaderNode>` **<** :ref:`Resource<class_Resource>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

Calculates a vector derivative within the visual shader graph.

Description
-----------

This node is only available in ``Fragment`` and ``Light`` visual shaders.

Properties
----------

+---------------------------------------------------------------------+-------------------------------------------------------------------------------+-------+
| :ref:`Function<enum_VisualShaderNodeVectorDerivativeFunc_Function>` | :ref:`function<class_VisualShaderNodeVectorDerivativeFunc_property_function>` | ``0`` |
+---------------------------------------------------------------------+-------------------------------------------------------------------------------+-------+

Enumerations
------------

.. _enum_VisualShaderNodeVectorDerivativeFunc_Function:

.. _class_VisualShaderNodeVectorDerivativeFunc_constant_FUNC_SUM:

.. _class_VisualShaderNodeVectorDerivativeFunc_constant_FUNC_X:

.. _class_VisualShaderNodeVectorDerivativeFunc_constant_FUNC_Y:

.. _class_VisualShaderNodeVectorDerivativeFunc_constant_FUNC_MAX:

enum **Function**:

- **FUNC_SUM** = **0** --- Sum of absolute derivative in ``x`` and ``y``.

- **FUNC_X** = **1** --- Derivative in ``x`` using local differencing.

- **FUNC_Y** = **2** --- Derivative in ``y`` using local differencing.

- **FUNC_MAX** = **3** --- Represents the size of the :ref:`Function<enum_VisualShaderNodeVectorDerivativeFunc_Function>` enum.

Property Descriptions
---------------------

.. _class_VisualShaderNodeVectorDerivativeFunc_property_function:

- :ref:`Function<enum_VisualShaderNodeVectorDerivativeFunc_Function>` **function**

+-----------+---------------------+
| *Default* | ``0``               |
+-----------+---------------------+
| *Setter*  | set_function(value) |
+-----------+---------------------+
| *Getter*  | get_function()      |
+-----------+---------------------+

A derivative type. See :ref:`Function<enum_VisualShaderNodeVectorDerivativeFunc_Function>` for options.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
