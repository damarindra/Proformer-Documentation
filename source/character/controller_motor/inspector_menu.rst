.. _doc_inspector_menu:

Inspector
=========

.. image:: /img/motor_inspector_menu.PNG

Inspector menu give you controller value, like movement, jumping, ladder, etc. In this section, not only build-in controller, but also
Custom Actions like Dash, Melee, and Gun.

**Health**

.. image:: /img/health_inspector.PNG

- Max Health -> Define character maximum health
- Health -> current character health
- Invisible Time -> total time character invisible when got damage / after die.
- Recover Time -> total time character can move after got damage
- Can Respawn -> define if character can respawning
- Respawn Time -> time needed to respawning
- Hit Clip -> Audio clip which play when got damage
- Flickering When Get Damage -> set true if you want character flickering when get damage
- Color flicker -> color flicker
- Transition Time Flickering -> time needed to switch between real color and flicker color
- Fade Out When Die -> Fading out when die
- Fade Out Smoothing -> Smoothing value when fading out

**Movement**

.. image:: /img/movement_inspector.PNG

- Move Speed -> speed movement
- Acceleration Time Grounded -> Acceleration time needed to reach move speed when grounded
- Acceleration Time Airbound -> Acceleration time needed to reach move speed when not grounded

**Jump**

.. image:: /img/jump_inspector.PNG

- Jump Permission -> set true to enable Jump Function
- Use Global Gravity -> Set true if you want to use global gravity (can be found at Edit/ProjectSettings/Physics)
- Max Jump Height -> Maximum jump height (only enable when UseGlobalGravity set to false)
- Min Jump Height -> Minimum jump height (only enable when UseGlobalGravity set to false)
- Time to jump Apex -> Time needed to maximum Jump Height (only enable when UseGlobalGravity set to false)
- Set To Global Gravity -> Set character gravity to global gravity (only enable when UseGlobalGravity set to false)
- Max Jump Velocity -> Maximum Jump Velocity (only enable when UseGlobalGravity set to true)
- Min Jump Velocity -> Minimum Jump Velocity (only enable when UseGlobalGravity set to true)
- Number Jump On Air -> Total jumping when not grounded
- Jump Clip -> Audio Clip will play when jumping
- Gravity -> readonly character gravity

**Ladder**

.. image:: /img/ladder_inspector.PNG

- Ladder Permission -> set true to enable Ladder Function
- Ladder Speed -> speed when climbing ladder
- Ladder Jump -> set true if your character can jumping while climbing ladder
- Unstick Ladder When Horizontal Move -> set true if your character can get off ladder when moving horizontally

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

**Crouch**

.. image:: /img/crouch_inspector.PNG

- Crouch Permission -> set true to enable Crouch Function
- Speed Crouch -> Movement speed when crouching
- Collider Scaller -> percentage scale body collider when crouching

**Custom Action**

.. image:: /img/customaction_inspector.PNG
