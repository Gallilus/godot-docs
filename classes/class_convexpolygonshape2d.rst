:github_url: hide

.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the ConvexPolygonShape2D.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_ConvexPolygonShape2D:

ConvexPolygonShape2D
====================

**Inherits:** :ref:`Shape2D<class_Shape2D>` **<** :ref:`Resource<class_Resource>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

Convex polygon shape for 2D physics.

Description
-----------

Convex polygon shape for 2D physics. A convex polygon, whatever its shape, is internally decomposed into as many convex polygons as needed to ensure all collision checks against it are always done on convex polygons (which are faster to check).

The main difference between a ``ConvexPolygonShape2D`` and a :ref:`ConcavePolygonShape2D<class_ConcavePolygonShape2D>` is that a concave polygon assumes it is concave and uses a more complex method of collision detection, and a convex one forces itself to be convex in order to speed up collision detection.

Properties
----------

+-----------------------------------------------------+-----------------------------------------------------------+--------------------------+
| :ref:`PackedVector2Array<class_PackedVector2Array>` | :ref:`points<class_ConvexPolygonShape2D_property_points>` | ``PackedVector2Array()`` |
+-----------------------------------------------------+-----------------------------------------------------------+--------------------------+

Methods
-------

+------+-------------------------------------------------------------------------------------------------------------------------------------------------------+
| void | :ref:`set_point_cloud<class_ConvexPolygonShape2D_method_set_point_cloud>` **(** :ref:`PackedVector2Array<class_PackedVector2Array>` point_cloud **)** |
+------+-------------------------------------------------------------------------------------------------------------------------------------------------------+

Property Descriptions
---------------------

.. _class_ConvexPolygonShape2D_property_points:

- :ref:`PackedVector2Array<class_PackedVector2Array>` **points**

+-----------+--------------------------+
| *Default* | ``PackedVector2Array()`` |
+-----------+--------------------------+
| *Setter*  | set_points(value)        |
+-----------+--------------------------+
| *Getter*  | get_points()             |
+-----------+--------------------------+

The polygon's list of vertices. Can be in either clockwise or counterclockwise order.

Method Descriptions
-------------------

.. _class_ConvexPolygonShape2D_method_set_point_cloud:

- void **set_point_cloud** **(** :ref:`PackedVector2Array<class_PackedVector2Array>` point_cloud **)**

Based on the set of points provided, this creates and assigns the :ref:`points<class_ConvexPolygonShape2D_property_points>` property using the convex hull algorithm. Removing all unneeded points. See :ref:`Geometry2D.convex_hull<class_Geometry2D_method_convex_hull>` for details.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
