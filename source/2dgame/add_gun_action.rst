.. _doc_add_gun_action:

Gun Action
==========

As far we have create player, follow path, and AI. Now we can add Gun to that, except Follow Path.
So, lets begin, first we create Projectile

Projectile
----------

Just like before, drag and drop your projectile sprite -> Right Click -> Proformer - Misc - Projectile -> Apply as Renderer -> Done
Then, see at inspector, we need to create Collider, expand Collider Section and click create button, choose collider as you want. I'm
using Circle Collider. Now just setup it properly.

Now, we jump to Projectile Properties Section. Setup it properly as always. I will tell you about Collide Mask, Horizontal Ray Count, Vertical Ray Count.
These 3 option will take care projectile colliding, such ground. Don't set Collide Mask with your damage target, because all take damage is listened by Trigger
Tag at Controller Motor component. You can follow my setup if you don't understand :

.. image:: /img/2d_tutor/projectile_inspector.PNG

Now we need to set the tag, first I want to create this projectile for Player Gun, so I need to set the tag with *Player Attack*, INCLUDING CHILD.
Then I duplicate the projectile gameobject by press ctrl + d, and the duplicate one set the tag with *Enemy*, because this projectile for Enemy AI.
Drag and drop 2 projectile gameobject to Project Window to make as prefabs.

Player Gun
----------

After creating Projectile, now we can add gun to our player. Just click Player, go to Inspector Menu, enable Custom Action GunAction.
Now scroll down and you found a new Gun Action Component.

.. image:: /img/2d_tutor/action.PNG

Open Action menu, drag and drop your Player Projectile Prefabs to Projectile field.
Then setup Projectile Position, you can setup it from field or click *Move* button and edit it in scene view. This is my setup

.. image:: /img/2d_tutor/gun_player.PNG

Then open Input Menu, expand it and drag and drop Player GameObject to target field. Set script field to 'Player (DI.Proformer.DIPlayer)', then set
Input to gunInput. Now test it by hit play, shoot using 'd' key.

.. image:: /img/2d_tutor/gun_input.PNG

.. note:: You can change input key from Edit - Project Settings - Input

AI Gun
------

Now, select your Enemy AI, and enable Gun Action from DI Character FSM or DI Controller Motor. Setup your GunAction Component like player gun. For Input,
you can drag and drop Enemy AI Game Object, select DICharacterFSM on script, and set input with gunInput. You can set the gun detection length at DICharacterFSM

.. image:: /img/2d_tutor/gun_ai.PNG
