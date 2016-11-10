.. _doc_create_enemy_follow_path:

Enemy Follow Path
=================

Drag and drop your Enemy Sprite, I'm using 'Bat' sprite, because bat is flying.
You can use basic Animator method for setup the animation, but I'm going with DISpriteAnim this time, because our Enemy Follow Path is can only moving.
So, select Bat GameObject, add a component name DI Sprite Anim. Go to Sprite Menu.

.. image:: /img/2d_tutor/sprite_anim.PNG

drag and drop all bat sprite on there, to add a new field, just click '+' button. And now go to Settings Menu

.. image:: /img/2d_tutor/sprite_anim_settings.PNG

Just setup it as you want, or you can follow my setup. If you want to see the animation, just press Play Test button.

After setting our Bat Renderer Game Object, now *Right Click* and select Proformer - Character - Follow Path Character
I'm just skip this section because I've explained it at :ref:`Create Player <create_character_2d>`

.. note:: Animator controller only used Idle state and Run state in Follow Path Character. (only if you not go with DISpriteAnim)

Configure Path
--------------

You can setup your points of movement with Path Component. To add a new Point, just click '+' button at Path Component.
As always, just try it out by yourself, but this is my configuration :

.. image:: /img/2d_tutor/enemy_path.PNG

Configure Follow Path
---------------------

Follow Path Character using Follow Path Component to control the movement. Thats why your Motor Inspector is only show Health property.
Setup your follow path as you want, for my configuration is look like these :

.. image:: /img/2d_tutor/follow_path_enemy.PNG

Make it Giving Damage to Player
-------------------------------

Go to setup menu, I haven't explain it, Give Damage and Impactable.

**Give Damage**, enable it now to make this Game Object giving damage. configure it as you want, this is my setup :

.. image:: /img/2d_tutor/give_damage.PNG

**Impactable**, enable it now to make this Game Object giving Impact to other object. config it as you want, this is my setup :

.. image:: /img/2d_tutor/impactable.PNG

Now, set our GameObject layer and tag to Enemy, **IMPORTANT : INCLUDING CHILD**. Navigate to **Player** GameObject, select Trigger Menu, add a new Give Damage
tag and Impactable tag, then set it as Enemy.

.. image:: /img/2d_tutor/trigger_player.PNG


Hit play and try it out, try to touch player with enemy. we've done here, you can continue to :ref:`Create Enemy AI <create_enemy_ai>`
