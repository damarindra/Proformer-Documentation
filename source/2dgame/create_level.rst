.. _doc_create_level:

Create Level
============

In this part, I'm not explaining to much because proformer is not *Level Creator Plugin*. I'm just explaing about creating ground and level bounds.

Ground
------

In Proformer, ground is an object which character type can step on. There is 2 type ground, *solid ground* and *one way ground*.

**Solid Ground**, you can make it by adding *Collider2D* to gameobject set the layer as *Ground*. Remember our World Type is 2D, only *Collider2D* works now.

**One Way Ground**, same as *Solid Ground*, but you need to set the tag as *One Way* now. What the difference? You can pass One Way Ground when jumping, and
you can pass it by jumping down.

So I will setup my current level look like these.

.. image:: /img/2d_tutor/level0.PNG

Level Bounds
------------

If you haven't read :ref:`Level Bounds <level_bounds>`, read it first.

So, because our World Type is 2D, we can only using one direction, right and left or we can say only Horizontal and Vertical, without Forward.
I'm not locking Level Bounds Points in 2D currently, because I need some suggestion, do I need to lock these? Please send your answer.

Back to tutorial, you can drag drop your Level Bounds point to set your level path. And you can set Top and Bottom from Inspector menu.
Mine will look like these

.. image:: /img/2d_tutor/level_bounds.PNG
