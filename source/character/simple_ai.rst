.. _doc_character_simple_ai:

Character Simple AI
===================

To create Simple AI, first things what must you do is create Character Simple AI from create menu.
I'm not planning to re-explain Setup and Inspector sections, because that was exactly same as Player.
So lets we move into Proformer Character AI Component. see picture

.. image:: /img/simple_ai_inspector.PNG

First things what must you do is set true Move Permission.

**Detection**

Hole detection and Wall Detection is option for take action after hole is detected, there is 6 option you can choose, there is Stop, Reverse Direction, Don't Stop, Jumping, Jumping_Stop, Jumping_Reverse

- Stop -> character will stop moving
- Reverse Direction -> character will reverse the direction
- Dont Stop -> ignore anything, just moving.
- Jumping -> will do jump
- Jumping_Stop -> first option is jumping, but if when calculate jumping target fail, then do stop action
- Jumping_Reverse -> first option is jumping, but if when calculate jumping target fail, then do Reverse action

**Offset Hole Detector Position** -> where hole detector started.

**Offset Wall Detector Length** -> ray length when detecting wall

**Move Range** -> Random time moving

**Idle Range** -> Random time idling

**State Watcher** -> For debuging
