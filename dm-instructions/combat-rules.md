# Combat Rules

OSRIC combat is round-based (1 round = 1 minute, subdivided into 10 segments) using THAC0 and
descending Armor Class. Full details: `osric-srd/markdown/12 time movement combat.md`.

## Sequence of a Round

1. **Declare actions** (spellcasting, retreat, and other segment-sensitive actions are declared first)
2. **Determine initiative** — roll 1d6 per side (or per combatant, if using individual initiative);
   lower result acts first. Re-roll each round.
3. **Resolve segments in order**: missile fire, spellcasting completion, movement, melee
4. **Melee/missile attacks resolve**: attacker rolls d20 + modifiers vs. target AC using THAC0
5. **Apply damage, check morale** for affected monsters/NPCs as needed
6. **Next round**

## THAC0 and To-Hit

- THAC0 = "To Hit Armor Class 0" — the d20 roll a character needs to hit AC 0.
- To hit AC *N*: needed roll = THAC0 − N (lower AC is better/harder to hit; negative AC is possible
  at high levels or with magic armor).
- A natural 20 always hits; a natural 1 always misses (house-rule variants may apply — confirm with
  the table before assuming).
- Show the math when resolving monster/NPC attacks: `[Orc attacks: THAC0 19, roll 14 = 14 vs AC 6 → hit, 1d8 dmg]`

## Attacks Per Round

- Most characters and 1+ HD monsters get 1 attack/round unless a class/monster entry states otherwise.
- Fighters (and sub-classes) gain extra attacks at higher levels (typically 3/2 at name level, 2/1 at
  high level) — confirm exact levels in the class tables.
- Creatures with under 1 HD may grant multiple attacks to a single attacker per round per the class
  tables (e.g. fighters vs. 1 HD or less).

## Saving Throws

Five categories, each with a target number by class and level (see class tables in
`osric-srd/markdown/`): **Paralyzation/Poison/Death**, **Petrification/Polymorph**, **Rod/Staff/Wand**,
**Breath Weapon**, **Spell**. Roll d20 ≥ the listed number to succeed. Always state which category
applies and let the player roll.

## Morale

NPCs and monsters check morale (2d6 vs. a morale rating) when first taking casualties, when a leader
falls, or when facing overwhelming odds. Failure means fleeing, surrendering, or routing — play it
out in character, don't just narrate "they flee" without letting players react.

## Surprise

Roll 1d6 per side (surprise on 1–2, or per monster entry if it differs) at the start of an encounter
before normal initiative. A surprised side loses actions for the surprise segments/round(s).

## Weapon Speed Factor & Weapon vs. Armor Type

Optional/advanced OSRIC rules — use weapon speed factor to break initiative ties, and weapon vs. armor
type adjustments for granular to-hit modifiers by weapon/armor combination. Use these only if the table
opts in; they add realism at the cost of speed.

## Death & Dying

- 0 hp: unconscious, dying (specific rules for negative hp thresholds — confirm table's variant, e.g.
  death at −10 hp vs. death at 0 hp is a common house-rule divergence).
- Track hit point loss precisely; OSRIC does not use hit point "milestones" — a single bad round can kill.
