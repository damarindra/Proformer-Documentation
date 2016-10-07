.. _doc_follow_path:

Follow Path Character
=====================

What must you do at the beginning is choose Character - Follow Path from create menu. Basically, create a character is not much diferent.
So I think I don't need to re-explaine Setup and Inspector Sections. Okay I will start from configuring Path.

Let see this picture

.. image:: /img/path_inspector.PNG

You can see there is 2 new component, **Path** and **Follow Path**. Path is a class for keeping a bunch of information position.
Follow Path is a class for controlling the movement. That was diferent with Player Character and Character AI which
movement controlled by Proformer Controller Motor.

Path
----

- You can see Path have a list of Position. The position here is following with Level Bounds, so the value range is between 0 - 1.
- Then there is **Level Path** field stand for where gameobject placed.
- And the last field is **Looping**. set true if you want set looping path.

Follow Path
-----------

- **speed** for movement speed.
- **wait time**, the movement will wait when reach each point.
- if you want smooth movement, set some value at **Ease Amount**.
- **Use Look At**, set true if you want the gameobject facing the right direction.
- set the **Loop Mode** as you want, ping-pong or once?
- Then the last thing **Execute Mode**, if you want to set the movement at the start, just set the value to Start. If you want execute the movement at specifics condition, just set **Loop Mode** to CALLMETHOD. You can activate by calling FollowPath.Execute(), if you want de-activate just call FollowPath.StopExecute()

So that was all for Follow Path Character. If you want to watch video tutorial, you can visit :ref:`Video Character Creation <character_creation>`.
