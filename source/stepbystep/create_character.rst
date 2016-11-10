.. _doc_create_character:

Character Creation
==================

There is 3 Character Type : Player, FSM, Follow Path
I will not explain what the difference about those things, I'm sure you know about that.

When creating character, you must complete Setup Menu (DIProformerMotor).

Setup
-----

**Position**, In this section, you can see only 1 field *Level Path Position*. This field
will set your current Object position relative to *Level Path*. You can read :ref:`Level Bounds <level_bounds>`
for more info about Level Path.

**Renderer**, If you haven't setup anything on renderer from 'Create New' Window, you can found this situation :

.. image:: /img/inspector/renderer_inspector.PNG

but, if you have setup renderer on 'Create New' Window, you will have this option. Basically this option
will appear when Renderer is applied.

.. image:: /img/inspector/renderer_applied_inspector.PNG

This option only resume from Renderer GameObject Inspector, you can change position directly, without focusing your
renderer object.

**Collider**, I'm sure you know what about Collider section. Yes, for setting up our Collider, hehe.
But the important point about collider is, do not edit center / offset of collider.
you ask why? answer is, when rotating / fliping character, collider will flip too right?
so if you don't want bug appear because of rotation, just set the center / offset to zero.

When you asking 'But I want to set up my collider position to fitting my renderer', I will answer
'You can setup your renderer position according to collider, right?'. And I've create a *Move* button
inside renderer Option. So problem solved.

Inspector
---------

Why the menu name is 'Inspector'? I'm still don't know which name better for this menu. In Inspector Menu, you can find a lot of option for controlling character, such Health, Moving, Jumping, etc.

.. image:: /img/inspector/motor_inspector.PNG

Trigger
-------

Trigger menu, controll almost all trigger event in Character, such Taking Damage, Impact, Picking Item, and Stomping.
For example you have an obstacle which giving damage to player, so you need to add one Take Damage Tag and set it to obstacle tag.

.. image:: /img/inspector/trigger_inspector.PNG
