.. doc_player:

Player (step-by-step)
=====================

If you want to create character, what you need is sprite/model and animation. If you have one and ready to create player, so lets do it.

Setup
-----

.. raw:: html

    <div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; height: auto;">
        <iframe src="//www.youtube.com/embed/TIvgSFZdYjk" frameborder="0" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"></iframe>
    </div>

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

Configure the movement
----------------------

- Lets choose Inspector menu.
- 
