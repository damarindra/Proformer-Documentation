.. _doc_create_enemy_ai:

Create Enemy AI
===============

Let me say Character AI instead of Enemy AI, because in Proformer you can set any
of character type to Enemy (except Player) and what I know about enemy is an antagonis actor.

Character AI is a character which can control by itself. You can make it as Enemy or Friendly.
In this part I only explain to make it as Enemy, that was why the title is Create Enemy AI.

So, what you need is just regular things like before, drag and drop sprite (I'm using dragon) to hierarchy, right click, Proformer - Character - Character AI.

Skip Setup Part.....

So, After completing setup section, I will tell you about what Character AI can do. Character AI can only Moving and Shooting. So the animator
animation state is only using Idle, Moving, Jumping, and Shooting. Skipping Setup the Animation and Animator part.....

Also, Inspector Properties only need to config Health, Movement, Jumping, and CustomAction - Gun (skip the gun at this part. will explain it another part)

.. image:: /img/2d_tutor/character_ai_motor.PNG


Character FSM
-------------

Character FSM is a component which controlled the character, you can say Character FSM is a brain.

**Movement AI**, this section will control the movement. You can config action when meet hole or wall. Then you also can config
movement time and idle time. AI is controlled using FSM method, I'm still learning about this method. I can say, this AI is not perfect now,
need a lot of feedback of you guys. You can follow my configuration :

.. image:: /img/2d_tutor/movement_ai_inspector.PNG

Make it as Enemy
----------------

Go to setup menu, I haven't explain it, Give Damage and Impactable.

**Give Damage**, enable it now to make this Game Object giving damage. configure it as you want, this is my setup :

.. image:: /img/2d_tutor/give_damage.PNG

**Impactable**, enable it now to make this Game Object giving Impact to other object. config it as you want, this is my setup :

.. image:: /img/2d_tutor/impactable.PNG

Now, set our GameObject layer and tag to Enemy, **IMPORTANT : INCLUDING CHILD**. Navigate to **Player** GameObject, select Trigger Menu, add a new Give Damage
tag and Impactable tag, then set it as Enemy.

.. image:: /img/2d_tutor/trigger_player.PNG
