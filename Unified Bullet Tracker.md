# Unified Bullet Tracker
The UBT stores the state of all projectiles and is responsible for determining their positions and detecting collisions.

## Projectile State
A projectile contains the following information:
- Trajectory: Kepler parameters
- [[Damage Model Data]] (ref)
- [[Render Data]] (ref)

Projectiles share damage model and render data based on the ammunition and weapon which created them.

## Position
Each frame, the position of each projectile is calculated and, with the previous frame's position, passed to the [[Renderer]] described by the projectile's render data. The calculation is a [[Kep2Cart|Kepler to Cartesian coordinate transform]].

## Collision Detection
A ray is cast from the previous frame's position to the current frame's position. Collisions thus obtained are passed to the [[Damage Model]] described by the projectile's damage model data.