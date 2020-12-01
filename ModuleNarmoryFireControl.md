# ModuleNarmoryFireControl
The Fire Control part module is responsible for generating firing solutions for associated [[ModuleNarmoryBattery]]s on assigned targets. Solvers are expected to be extended to account for e.g. evading targets or targeting of specific parts.

## List of Solvers
- Manual: The player's cursor drives the bearing directly.
- Naïve: The bearing points directly at the target.
- Simple: An intercept is generated assuming flat space and constant velocities.
- Orbital: An intercept is generated assuming orbital effects and a ballistic target.
- Dynamic: An intercept is generated taking the target's current acceleration and angular velocity into account.