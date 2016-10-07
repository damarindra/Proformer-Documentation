.. doc_player:

Player (step-by-step)
=====================

If you want to create character, what you need is sprite/model and animation. If you have one and ready to create player, so lets do it.
If you confused, you can watch video of Character Creation, visit here :ref:`Video Character Creation <character_creation>`.

Setup
-----

- First, click create on hierarchy, then choose Proformer -> Character -> Player

.. image:: /img/create_player.PNG

- Then a new GameObject called player created. First things what you need to do is complete the setup section.
- Click create button on collider section. Then a new Collider will apears as a child of Player GameObject, named Body. You can configure the size of Body later.

.. image:: /img/create_body.PNG

- After that, we need to add renderer to our Player GameObject. So, if you going for 2D games, which you have a sprite, what you must do is drag and drop your sprite to hierarchy, so it will become as GameObject. if 3D you don't need to do this because model is automatically turn as GameObject.
- Then drag and drop to the Renderer Object field at Renderer Section.

.. image:: /img/create_renderer.PNG

- You can see, now Apply button is active, just click it!
- Then you can configure the other options like body size, renderer position, and the others now.
- The last things is create animator controller. What must you do is click Add Animator Button  inside renderer sections.
- Then a new field Animator Controller is appear. click create button on the right side of Animator Controller field
- A new window will apears to set the Animator Controller locations.
- This create action will create a new Pre-configure Animator Controller. So what you must do is just assign Animation clip to each Animation State in Animator Controller.

Configure the movement
----------------------

- Lets choose Inspector menu.
- There is a bunch of options, so configure it as what you need. You can see at :ref:`Inspector Menu <doc_inspector_menu>` for more details.
- After complete setting up at Inspector Menu, so just try it first. Hit play button. Don't forget to add a new ground object, just create a new gameobject with a collider (if 2D use collider2D), then set layer to Grounds.

Trigger Menu
------------

Trigger menu contains a list of trigger listener. for more information just visit :ref:`Trigger Menu <doc_trigger_menu>`
