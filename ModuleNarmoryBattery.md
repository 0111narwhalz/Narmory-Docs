# ModuleNarmoryBattery
The Battery vessel module is used to group [[ModuleNarmoryTurret]]s and [[ModuleNarmoryWeapon]]s. It is responsible for distributing the target bearing to included turrets and managing individual Weapon triggers.

## Grouping
A Battery can contain Turreted or fixed Weapons, but not both. Batteries are expected to operate as single units, and should be homogenous in terms of included Weapons (Turrets with similar attached Weapons are considered homogenous). Groups are adjusted via an interface visible in the Action Groups area (editor and flight).

## Distribution of Target Bearing
Given a target bearing and optionally a range, the Battery calculates a bearing for each of its Turrets. The range is used to adjust for convergence.
This feature is disabled for fixed Batteries.

## Weapon Triggers
When given the fire command, the Battery generates a set of Weapons within its pointing tolerance. According to its fire mode, it issues fire events to each Weapon. An unfirable weapon never blocks firable weapons from firing.

## Firing Modes
- Synchronized Fire: All Weapons fire at once.
- Sustained Fire: Weapons fire at the maximum rate which permits each to be reloaded before being asked to fire again.
- Burst Fire: Weapons fire at a rate elevated from Sustained Fire. This rate is adjustable in the Battery interface.
- At Will: Weapons fire as soon as they are within pointing tolerance and loaded.