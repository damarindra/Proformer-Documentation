.. _doc_setup:

Setup
=====

.. image:: /img/motor_setup_menu.PNG

Setup menu contains configurable Game Object, like Position, Collider, Renderer, Animator, etc.
When you create a new Character Type, you must be complete Setup Sections.

**Position**

.. image:: /img/position_inspector.PNG

- Level Path Position -> index level path where gameobject is placed.
- Raw Horizontal -> raw horizontal is between 0 - 1.
- Raw Vertical -> raw vertical is between 0 - 1.

Confuse? Position in this part is means position relative to Level Bounds. Please read Level Bounds sections.

Simple Explaination is, Level Bounds has an array of Level Path. If raw horizontal is 0,
that means your horizontal position is equal to LevelPath.from.
and if raw horizontal is 1, that means your horizontal position is equal to LevelPath.to.
same as vertical, if 0, then your vertical position is equal with LevelBounds.bottom, and otherwise.

**Controller**

.. image:: /img/controller_inspector.PNG

- Horizontal Ray Count -> How many ray will cast horizontally
- Vertical Ray Count -> How many ray will cast vertically
- Slope limit -> maximal angle value character can climb slope.

**Body Collider**

.. image:: /img/body_collider_inspector.PNG

- Body Collider -> Object field body collider
- Width -> body collider width
- Height -> body collider height
- Depth -> body collider depth

**Renderer**

.. image:: /img/renderer_inspector.PNG

- Renderer Object -> Target Renderer GameObject.
- Character Renderer -> Renderer Component at Renderer Gameobject.
- Position -> Local Position of Renderer GameObject
- Rotation -> Local Rotation of Renderer GameObject
- Scale -> Local Scale of Renderer GameObject
- Animator Controller -> Animator Controller of Renderer

**Wall Sliding**

.. image:: /img/wallsliding_inspector.PNG

- Wall Slide Permission -> set true to enable Wall Slide Function
- Wall Jump Climb -> jump speed when wall jump climb (did you know megaman, yes like that)
- Wall Jump Off -> unstick wall slide speed
- Wall Leap -> wall leap speed, different with Jump Climb, leap is jumping at the opposite direction
- Wall Slide Speed Max -> speed wall sliding down
- Wall Stick Time -> total time sticking when your direction input is going opposite of direction wall.
- Unstick When Dir Touch Up -> set true if you want unstick when you don't pressed direction button
- Reverse Wall Slide -> Reverse the renderer object direction.

**Give Damage and Impactable**

.. image:: /img/givedamage_impactable_inspector.PNG

Will active when gameobject is set to enemy
