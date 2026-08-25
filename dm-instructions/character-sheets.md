# Character Creation & Sheets

Full ability/race/class rules: `osric-srd/markdown/02 ability scores and races.md`,
`03a character classes assassin-illusionist.md`, `03b character classes magic user-multiclass.md`.

## Creation Steps

1. **Roll ability scores**: 3d6 in order (Strength, Intelligence, Wisdom, Dexterity, Constitution,
   Charisma) is the default OSRIC method. Confirm with the table if using an alternate method (4d6
   drop lowest, point buy, etc.) before deviating.
2. **Choose race**: Human, Dwarf, Elf, Gnome, Half-Elf, Halfling, Half-Orc. Each race has ability
   score minimums/maximums, class/level restrictions, and special abilities (infravision, resistance
   to magic, detect secret doors, etc.).
3. **Choose class**: Fighter, Paladin, Ranger, Cleric, Druid, Magic-User, Illusionist, Thief, Assassin
   (and multi-class/dual-class combinations, where race/rules allow). Race determines which classes
   and level limits are available.
4. **Note prime requisite(s)**: Each class has one or more prime requisite ability scores. A high
   prime requisite score grants an XP bonus (typically +5% or +10%); a low score can impose a penalty.
5. **Determine hit points**: Roll class hit die + Constitution modifier. Level 1 characters typically
   take max hit points at the table's discretion — confirm the house rule.
6. **Alignment**: One of the nine alignments (Lawful/Neutral/Chaotic × Good/Neutral/Evil).
7. **Starting equipment & gold**: Roll starting gold per class (e.g. 3d6×10 gp for fighters — see
   equipment tables), then purchase equipment from `osric-srd/markdown/04 alignment money equipment.md`.
8. **Calculate derived stats**: THAC0 (by class/level), Armor Class (base 10 − armor/shield/Dex
   bonus), saving throws (by class/level), movement rate.

## Race/Class Level Limits

Demi-human characters (Dwarf, Elf, Gnome, Half-Elf, Halfling, Half-Orc) have **maximum levels** per
class, often tied to ability scores (e.g. exceptional Strength can raise a Dwarf fighter's level cap).
Only humans are uncapped. Always check the race entry before leveling a demi-human past its normal cap.

## Exceptional Strength

Fighters (and sub-classes) with 18 Strength roll percentile dice (18/01–18/00) for exceptional
Strength, granting to-hit/damage bonuses beyond a flat 18. Non-fighter classes do not get this roll
even with 18 Strength.

## Character Sheet Contents

When displaying or storing a character (`campaigns/[name]/characters/[character].md`), include:

- Name, race, class(es), level(s), alignment, XP (current / needed for next level)
- Ability scores (with derived modifiers)
- AC, THAC0, hit points (current/max), movement rate
- Saving throw targets (all five categories)
- Class abilities/spells known or memorizable
- Equipment, encumbrance, gold
- Languages, henchmen/hirelings (if any)

## Leveling Up

On gaining a level: roll new hit die (+ Con modifier), update THAC0 and saving throws per the class
table, add new spell slots (for casters), and check demi-human level limits before applying.
