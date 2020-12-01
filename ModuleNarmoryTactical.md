# ModuleNarmoryTactical
The Tactical AI part module is responsible for interpreting the battlespace. It provides IFF and threat identification, target prioritization, fire authority, and evasion, and addresses all [[ModuleNarmoryFireControl]]s on its vessel.
At most one Tactical AI is permitted to be active on a given vessel. A priority is assigned to each Tactical AI; if this is insufficient, the part closest to the root in the vessel tree is selected; finally, the part with the smallest UID is selected.

## IFF and Threat ID

## Target Prioritization

## Fire Authority

## Evasion