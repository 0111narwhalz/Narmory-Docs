# ModuleNarmoryWeapon
The Weapon part module is responsible for emitting projectiles and consuming ammunition, as well as animating the part to which it is attached.

## Projectile Emission
When the Weapon receives a fire event, it adds a projectile to the [[Unified Bullet Tracker]] based on its own position, velocity, and orientation, as well as its muzzle velocity. To this projectile are attached a [[Damage Model Data]] and a [[Render Data]] by reference.

## Ammunition Consumption
When the Weapon emits a projectile, it subtracts its defined ammunition resource(s) from connected resource-storing parts. Preferably, it pulls all ammunition from one part, to avoid non-integer numbers of bullets.

## Part Animation
The Weapon module can animate the part to which it is attached, to display e.g. recoiling barrels or ammunition feeds.