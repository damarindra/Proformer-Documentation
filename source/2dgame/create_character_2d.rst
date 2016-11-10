.. _doc_create_character_2d:

Create Player 2D
===================

First of all, make sure you have an assets to follow this tutorial, if you don't have one, you can use `this one <www.http://opengameart.org/content/platform-pixel-art-assets>`_ (CC0)
Okay, let's get started.

Manage All Assets
-----------------

After importing all assets to Unity, we need to cut our sprite. This basics things in unity, if you know you can skip this section.
Navigate to your Sprite assets

.. image:: /img/2d_tutor/sprite_assets.PNG

Select player sprite, see at inspector window and setup look like this :

.. image:: /img/2d_tutor/sprite_inspector.PNG

Click *Apply*, then click *sprite editor*. We need to cut our sprite, I will not doing manually,
we can use 'Slice' method, so click *Slice* button, and make sure your setup look like this :

.. image:: /img/2d_tutor/slice_sprite.PNG

Now, click *Slice* buton and *Apply*.

For other sprite, you can do it like that, so I don't need to re-write this section.

Create Player Game Object
-------------------------

After slicing all player Sprite, select one of those sprite and drag and drop to scene view / hierarchy.
Now, we have player sprite in Scene View. Go to hierarchy and *Right Click* your player sprite, select Proformer - Character - Player

.. image:: /img/2d_tutor/right_click_player.PNG

A **Create New** window will appears. Make sure renderer field is your player sprite gameobject. If not, just drag and drop your player sprite gameobject
to renderer field. Now click *Apply As Renderer*. This action will make your Player Sprite as a child of Player GameObject. Just click done now.

.. image:: /img/2d_tutor/create_new_window.PNG

Now, navigate to Inspector Window. Select **Setup** menu, and configure our create our collider. Just expand *Collider* section, and click *create* button.
A new GameObject named *Body* created as a Child of Player GameObject. We can configure our collider directly from Player GameObject or go to Body GameObject.

.. note:: Editing offset / center of Collider component will make your character buggy when fliping, only when flip at the front of ground. Instead editing offset / center of Collider, we can move our Renderer GameObject.

You can edit your collider size now. After that, you can alligning your Renderer GameObject to your collider.

After that, you can see *Add Animator* button right? just click that button to Add Animator Component at Renderer GameObject. if you don't found that button,
that means your character has Animator Component. A new field and button appears now, just click *create* button, new window will show and navigate your Animator Controller folder path.
in my case, my path is /Assets/Tutorial/Animation/Player/Player.controller. Now check your animator controller by select renderer game object, and open Animator window (Window/Animator)
As you can see, Pre-setup animator controller is avaiable to your player. Just open Base Animation by double clicking.

Create Animation and Assigning Animation
--------------------------------------

Because we using sprite, we can create our animation in Unity Editor. Open Animation window (Window/Animation) and click *Create* button (make sure your selected GameObject is Renderer GameObject).
I'm begin with run animation, just name it as Run. Then I will set it look like these

.. image:: /img/2d_tutor/animation_run.PNG

Do it with other animation such Idle, Jump, Shoot.

Now I'm going to Assigning all animation to animator controller. Make sure your selected gameobject is Renderer GameObject, open Animator Window, and assign
our Animation to each state. Just click Idle state at Animator, then see at inspector, you can found Motion field, drag and drop Idle Animation to Motion Field.
Do it to all Animation we've created.

So we've done now. Just hit play and try it. If you haven't any ground yet, just create a new gameobject and add BoxCollider2D Component, then set layer as Grounds.

Configure Motor Properties
--------------------------

Now we can setup our motor properties, such Move Speed, Jump height, etc. Just open *Inspector* Menu at Motor Component.
Expand each of those section and set the values. You can follow my configured properties or not, it's up to you now. For custom action do not activate now,
just leave it unchecked.

.. image:: /img/2d_tutor/motor_properties.PNG

Now just hit play at test it. And this part is done here. You can go to :ref:`Create Level <create_level>`.
