.. _doc_set_as_enemy:

Set Character As Enemy
======================

When you create Character (except player) will set as whitelist, you can say, the character is not as enemy.
So we need to set a character as Enemy, how to do this? Select a Character at Hierarchy, then select Set As Enemy at menu Assets/Proformer/Set Selected As Enemy.
This will be automatically set the character as Enemy.

Remember Option Give Damage and Impactable at Setup Menu? now those options is enable, you can setup it.

**Questions**

Q : Why character not taking damage to player attack?

A : Don't forget to configuring Take Damage Tag at Trigger Menu. Add a new one and set as target Tag. (ex : PlayerAttack)
