# Damage Model
The Damage Model interprets a collision sequence and, with an attached [[Damage Model Data]], applies damage to involved parts. Damage models may affect multiple parts in a single frame.

## List of Damage Models
- [[DamageDebug]]: For debug purposes. Depending on data, can apply fixed damage, instantly destroy a part, or signal only.
-  [[DamageKinetic]]: For inert kinetics at mundane velocities. Covers the velocity spectrum from "bumping" to multiple km/s hypervelocity, but is not appropriate for Mm/s or relativistic impacts.