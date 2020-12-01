# ModuleNarmoryTurret
The Turret part module is responsible for laying co-attached [[ModuleNarmoryWeapon]]s and animating turret geometry.

## Gun Laying
Given a bearing in worldspace, the Turret will rotate until its co-attached Weapons are aligned with it. They will hold this attitude until issued either a new bearing or a stow command, in which case they return to a neutral position.

## Animation
The Turret animates the part to which it is attached, laying the co-attached weapons to the target bearing.