# OSRIC — Master Index

*OSRIC — master index of every spell, monster, and magic-item name to the transcription file that carries its full entry. Built batch 18, from the audited entry rosters (`01 lists.md`, each source file's own header line, and the corresponding batch record).*

**⚠ Provisional — built before the audit backlog closed.** As of batch 18, 22 of the 33 transcribed source files (16a through 32) have not been through an independent audit pass — see `03 file manifest.md`'s status table. The project's own job order calls for the master index to be *"Built last, from the **audited** entry rosters"*; building it now, against the full-but-not-fully-audited set, is a deliberate exception made on the owner's explicit instruction for batch 18 ("NO AUDIT; JUST THE 3 ITEMS WE MENTIONED"), not a discovery that the audit-first sequencing no longer applies. Audits have found real roster-level problems before, not hypothetically: audit batch 4 corrected file 13's mis-tallied header counts and found file 14b missing an entire column of content on book p.155. If a later audit finds something like that in one of the 22 unaudited files below, this index will need a follow-up patch, because it will have been built from a roster that turned out to be wrong. Every File/Page cite below reflects the source file exactly as delivered; this index-building pass did not independently re-verify any of them against the PDF.

**Routing table — the one exception to this project's no-contents-block rule.** Every verbatim transcription file carries no contents block, no table of contents, and no anchor links, per `01 transcription template.md`'s standing convention — the consumer is a Claude instance that fetches one whole file and reads all of it, and a contents block would be duplicated content that costs tokens on every fetch and buys nothing. This file is different: its entire job is routing — *which file do I fetch for "Owlbear"?* — so it is allowed to be exactly the lookup table every other file is forbidden from being. State this here so nobody mistakes this file's structure for a violation of that rule.

## How to use this file

Look up a name in the tables below. The **File** column gives a short code; resolve it against the legend immediately below to the actual filename. The **Page** column is the book's own page number for where the entry's full description *begins* in that file — this is usually, but not always, the same page the book's own front-matter list cites (see the Ring of Spell Turning entry, under Rings, for a case where it is not). A non-empty **Note** flags something about that specific row worth reading before you trust it — a printed-error correction, an unresolved owner-decision conflict, or an unusual routing.

## File code legend

| Code | Filename |
|---|---|
| 06a | `06a spells cleric aerial servant-hold person.md` |
| 06b | `06b spells cleric holy word-word of recall.md` |
| 07 | `07 spells druid.md` |
| 08 | `08 spells magic user aff-for.md` |
| 09 | `09 spells magic user fre-per.md` |
| 10 | `10 spells magic user pha-wri.md` |
| 11 | `11 spells illusionist.md` |
| 17a | `17a monsters statistics men demi-humans.md` |
| 17b | `17b monsters humanoids giants.md` |
| 18 | `18 monsters dragons and demons.md` |
| 19 | `19 monsters devils dinosaurs golems.md` |
| 20 | `20 monsters sylvan and undead.md` |
| 21 | `21 monsters animals.md` |
| 22a | `22a monsters other a-cat.md` |
| 22b | `22b monsters other cen-gar.md` |
| 23a | `23a monsters other gel-mer.md` |
| 23b | `23b monsters other min-rem.md` |
| 24 | `24 monsters other roc-z.md` |
| 25 | `25 treasure coin gems potions scrolls.md` |
| 26 | `26 rods staves wands armour swords.md` |
| 27 | `27 miscellaneous magic a-gog.md` |
| 28 | `28 miscellaneous magic gog-z.md` |
| 29a | `29a rings and cursed items i.md` |
| 29b | `29b cursed items ii and artifacts.md` |

## What is not indexed here, and why

Not every transcribed file fits the name-indexed pattern this index uses, and not every file is in scope for it at all. Handled as explicit exceptions, not silently:

- **00 front matter, 01 lists, 33 licence** — front matter, the source roster itself, and legal text. No spell/monster/magic-item entries of their own to index; `01 lists.md` is this index's own audited source, not something it indexes.
- **02, 03a, 03b, 04** (Chapter I, Creating a Character) — ability scores, races, classes, alignment, money, equipment. Player-facing character-creation material, not spell/monster/magic-item entries.
- **05** (spells overview) — the spells chapter's introductory rules and mechanics sections. The spell *entries* themselves are in 06a through 11, which are indexed below; 05's own sections are not.
- **12, 13, 14a, 14b, 15, 16a, 16b** (Chapters III–IV, How to Play / Dungeons, Towns and Wildernesses) — rules text, hireling and henchman rules, the worked example dungeon and sample play session, dungeon generation tables, and encounter tables. None of these carry named spell/monster/magic-item entries in the indexed sense (the encounter *tables* in 16a/16b reference monster names that already have their own full entries in the Chapter V files, indexed below under Monsters).
- **30** (compiled tables, Appendix A) — 38 table and section headings (class Saving Throw/To Hit pairs, Thief Skills tables, the Melee/Missile Weapon tables, the Monster Equivalent Level table, and so on), not named creatures or magic items. The manifest itself flags this file as likely feeding the index differently than the chapter files, if at all — it does not fit the name-indexed structure and is not forced into it here.
- **31** (afterword) — eleven paragraphs of prose, no discrete entries.
- **32** (index) — itself an index of the book's own printed page numbers (a general index of terms, plus a nested Index of Tables), not of spell/monster/magic-item names. More useful as a cross-check against this file than as a source for it — see the count reconciliation below.

## Count reconciliation

This index carries **1,050 entries** (414 spells, 292 monsters, 344 magic items) against `01 lists.md`'s audited **1,048** (414 spells, 292 monsters, 342 magic items). The gap is fully accounted for, not incidental:

- **+2, Miscellaneous Magic — Headband of Intellect and Portable Hole.** Both are genuinely printed and described in file 28's body text (found in batch 14: independently confirmed against the raster at both locations) but are absent from the book's own front-matter List of Magic Items. `01 lists.md` is not at fault for this — it faithfully transcribes what the book's own front-matter list actually contains; the front-matter list itself is what's incomplete. Both are indexed below, each flagged with a Note.

Every spell (414 of 414) and every monster (292 of 292) in the audited roster maps to exactly one row below with no adjustment needed.

## Cross-references and synonyms — the convention used here, stated explicitly

The book gives several entries an alternate name in parentheses directly in its own front-matter list — "Bandit (Brigand)," "Buccaneer (Pirate)," "Dervish (Nomad)," "Caveman (Tribesman)," and others. These print as **one entry**, not two cross-referenced headings, so this index gives each a single row under its primary printed name, parenthetical included exactly as printed, rather than adding a second "see" row under the alternate name. Nothing in this book's own three front-matter lists takes the form of a bare cross-reference (a hypothetical "Faerie Creatures — see Sylvan"); none were found while building this index. If one turns up in a future pass, the convention for it is: a second row pointing at the primary entry's own File/Page, with the Note column marked as a cross-reference — not folded silently into the primary row's page cite.

One monster is a genuine structural exception, not a naming one: **Dread Wraith** prints in the book's own List of Monsters out of sequence (after Yeti, pointing at page 372 — a confirmed leave-alone-list oddity, not something to correct), but its only appearance anywhere in the book's body text is as a stat block embedded inside the **Deck of Many Things** magic-item entry, in file 29b — it has no chapter-file entry of its own anywhere in the Monsters chapters. Indexed below under Monsters, filed at 29b, flagged accordingly, precisely so a reader searching Monsters for Dread Wraith is routed correctly rather than left to conclude it was missed.

---

## Spells

### Cleric

| Entry | Page | File | Note |
|---|---|---|---|
| Aerial Servant | 40 | 06a |  |
| Animate Dead | 40 | 06a |  |
| Animate Object | 41 | 06a |  |
| Astral Spell | 41 | 06a |  |
| Atonement | 41 | 06a |  |
| Augury | 41 | 06a |  |
| Blade Barrier | 42 | 06a |  |
| Bless* | 42 | 06a |  |
| Chant | 42 | 06a |  |
| Command | 42 | 06a |  |
| Commune | 42 | 06a |  |
| Conjure Animals | 43 | 06a |  |
| Continual Light* | 43 | 06a |  |
| Control Weather | 43 | 06a |  |
| Create Food and Water | 43 | 06a |  |
| Create Water* | 43 | 06a |  |
| Cure Blindness* | 43 | 06a |  |
| Cure Critical Wounds* | 44 | 06a |  |
| Cure Disease* | 44 | 06a |  |
| Cure Light Wounds* | 44 | 06a |  |
| Cure Serious Wounds* | 44 | 06a |  |
| Detect Charm* | 44 | 06a |  |
| Detect Evil* | 44 | 06a |  |
| Detect Lie* | 45 | 06a |  |
| Detect Magic | 45 | 06a |  |
| Dispel Evil* | 45 | 06a |  |
| Dispel Magic | 45 | 06a |  |
| Divination | 45 | 06a |  |
| Earthquake | 46 | 06a |  |
| Exorcise | 46 | 06a |  |
| Feign Death | 46 | 06a |  |
| Find the Path* | 46 | 06a |  |
| Find Traps | 46 | 06a |  |
| Flame Strike | 47 | 06a |  |
| Gate | 47 | 06a |  |
| Glyph of Warding | 47 | 06a |  |
| Heal* | 47 | 06a |  |
| Hold Person | 47 | 06a |  |
| Holy Word* | 48 | 06b |  |
| Insect Plague | 48 | 06b |  |
| Know Alignment* | 48 | 06b |  |
| Light* | 48 | 06b |  |
| Locate Object* | 49 | 06b |  |
| Lower Water* | 49 | 06b |  |
| Neutralise Poison* | 49 | 06b |  |
| Part Water | 49 | 06b |  |
| Plane Shift | 49 | 06b |  |
| Prayer | 50 | 06b |  |
| Pro. from Evil* | 50 | 06b |  |
| Pro. from Evil, 10 ft Radius* | 50 | 06b |  |
| Purify Food and Drink* | 50 | 06b |  |
| Quest | 51 | 06b |  |
| Raise Dead* | 51 | 06b |  |
| Regenerate* | 51 | 06b |  |
| Remove Curse* | 51 | 06b |  |
| Remove Fear* | 52 | 06b |  |
| Resist Cold | 52 | 06b |  |
| Resist Fire | 52 | 06b |  |
| Restoration* | 52 | 06b |  |
| Resurrection* | 52 | 06b |  |
| Sanctuary | 52 | 06b |  |
| Silence, 15 ft Radius | 53 | 06b |  |
| Slow Poison | 53 | 06b |  |
| Snake Charm | 53 | 06b |  |
| Speak with Animals | 53 | 06b |  |
| Speak with Dead | 53 | 06b |  |
| Speak with Monsters | 54 | 06b |  |
| Speak with Plants | 54 | 06b |  |
| Spiritual Weapon | 54 | 06b |  |
| Sticks to Snakes* | 54 | 06b |  |
| Stone Tell | 54 | 06b |  |
| Symbol | 55 | 06b |  |
| Tongues* | 55 | 06b |  |
| True Seeing* | 55 | 06b |  |
| Wind Walk | 55 | 06b |  |
| Word of Recall | 55 | 06b |  |

### Druid

| Entry | Page | File | Note |
|---|---|---|---|
| Animal Friendship | 56 | 07 |  |
| Animal Growth* | 56 | 07 |  |
| Animal Summoning I | 56 | 07 |  |
| Animal Summoning II | 56 | 07 |  |
| Animal Summoning III | 56 | 07 |  |
| Animate Rock | 57 | 07 |  |
| Anti-Animal Shell | 57 | 07 |  |
| Anti-Plant Shell | 57 | 07 |  |
| Barkskin | 57 | 07 |  |
| Call Lightning | 57 | 07 |  |
| Call Woodland Beings | 57 | 07 |  |
| Chariot of Fire | 58 | 07 |  |
| Charm Person or Mammal | 58 | 07 |  |
| Commune With Nature | 58 | 07 |  |
| Confusion | 58 | 07 |  |
| Conjure Earth Elemental* | 59 | 07 |  |
| Conjure Fire Elemental* | 59 | 07 |  |
| Control Temp. 10 ft Radius | 59 | 07 |  |
| Control Weather | 59 | 07 |  |
| Control Winds | 60 | 07 |  |
| Create Water | 60 | 07 |  |
| Creeping Doom | 60 | 07 |  |
| Cure Disease* | 60 | 07 |  |
| Cure Critical Wounds* | 60 | 07 |  |
| Cure Light Wounds* | 60 | 07 |  |
| Cure Serious Wounds* | 61 | 07 |  |
| Detect Magic | 61 | 07 |  |
| Detect Pits and Snares | 61 | 07 |  |
| Dispel Magic | 61 | 07 |  |
| Entangle | 61 | 07 |  |
| Faerie Fire | 61 | 07 |  |
| Feeblemind | 61 | 07 |  |
| Feign Death | 62 | 07 |  |
| Finger of Death | 62 | 07 |  |
| Fire Seeds | 62 | 07 |  |
| Fire Storm* | 62 | 07 |  |
| Fire Trap | 62 | 07 |  |
| Hallucinatory Forest | 62 | 07 |  |
| Heat Metal* | 63 | 07 |  |
| Hold Animal | 63 | 07 |  |
| Hold Plant | 63 | 07 |  |
| Insect Plague | 64 | 07 |  |
| Invisibility to Animals | 64 | 07 |  |
| Locate Animals | 64 | 07 |  |
| Locate Plants | 64 | 07 |  |
| Neutralise Poison* | 64 | 07 |  |
| Obscurement | 64 | 07 |  |
| Pass Plant | 64 | 07 |  |
| Pass Without Trace | 65 | 07 |  |
| Plant Door | 65 | 07 |  |
| Plant Growth | 65 | 07 |  |
| Predict Weather | 65 | 07 |  |
| Produce Fire* | 65 | 07 |  |
| Produce Flame | 65 | 07 |  |
| Pro. From Fire | 66 | 07 |  |
| Pro. From Lightning | 66 | 07 |  |
| Purify Water* | 66 | 07 |  |
| Pyrotechnics | 66 | 07 |  |
| Reincarnate | 66 | 07 |  |
| Repel Insects | 67 | 07 |  |
| Shillelagh | 67 | 07 |  |
| Snare | 67 | 07 |  |
| Speak With Animals | 67 | 07 |  |
| Speak With Plants | 68 | 07 |  |
| Sticks to Snakes* | 68 | 07 |  |
| Stone Shape | 68 | 07 |  |
| Summon Insects | 68 | 07 |  |
| Transmute Metal to Wood | 68 | 07 |  |
| Transmute Rock to Mud* | 68 | 07 |  |
| Transport via Plants | 68 | 07 |  |
| Tree | 69 | 07 |  |
| Trip | 69 | 07 |  |
| Turn Wood | 69 | 07 |  |
| Wall of Fire | 69 | 07 |  |
| Wall of Thorns | 70 | 07 |  |
| Warp Wood | 70 | 07 |  |
| Water Breathing* | 70 | 07 |  |
| Weather Summoning | 70 | 07 |  |

### Magic User

| Entry | Page | File | Note |
|---|---|---|---|
| Affect Normal Fires | 70 | 08 |  |
| Airy Water | 70 | 08 |  |
| Animal Growth* | 71 | 08 |  |
| Animate Dead | 71 | 08 |  |
| Anti-Magic Shell | 71 | 08 |  |
| Antipathy/Sympathy | 71 | 08 |  |
| Astral Spell | 71 | 08 |  |
| Audible Glamour | 71 | 08 |  |
| Blink | 72 | 08 |  |
| Burning Hands | 72 | 08 |  |
| Cacodemon | 72 | 08 |  |
| Charm Monster | 72 | 08 |  |
| Charm Person | 73 | 08 |  |
| Charm Plants | 73 | 08 |  |
| Clairaudience | 73 | 08 |  |
| Clairvoyance | 73 | 08 |  |
| Clenched Fist | 74 | 08 |  |
| Clone | 74 | 08 |  |
| Cloudkill | 74 | 08 |  |
| Comprehend Languages* | 74 | 08 |  |
| Cone of Cold | 75 | 08 |  |
| Confusion | 75 | 08 |  |
| Conjure Elemental | 75 | 08 |  |
| Contact Other Plane | 75 | 08 |  |
| Continual Light | 76 | 08 |  |
| Control Weather | 76 | 08 |  |
| Crushing Hand | 76 | 08 |  |
| Dancing Lights | 76 | 08 |  |
| Darkness, 15 ft Radius | 76 | 08 |  |
| Death Spell | 77 | 08 |  |
| Delayed Blast Fireball | 77 | 08 |  |
| Detect Evil* | 77 | 08 |  |
| Detect Invisibility | 77 | 08 |  |
| Detect Magic | 77 | 08 |  |
| Dig | 77 | 08 |  |
| Dimension Door | 78 | 08 |  |
| Disintegrate | 78 | 08 |  |
| Dispel Magic | 78 | 08 |  |
| Distance Distortion | 78 | 08 |  |
| Duo-Dimension | 78 | 08 |  |
| Enchant an Item | 79 | 08 |  |
| Enchanted Weapon* | 79 | 08 |  |
| Enlarge* | 79 | 08 |  |
| Erase | 79 | 08 |  |
| ESP | 80 | 08 |  |
| Explosive Runes | 80 | 08 |  |
| Extension I | 80 | 08 |  |
| Extension II | 80 | 08 |  |
| Extension III | 80 | 08 |  |
| False Trap | 80 | 08 |  |
| Fear | 81 | 08 |  |
| Feather Fall | 81 | 08 |  |
| Feeblemind | 81 | 08 |  |
| Feign Death | 81 | 08 |  |
| Find Familiar | 81 | 08 |  |
| Fire Charm | 82 | 08 |  |
| Fire Shield | 82 | 08 |  |
| Fire Trap | 82 | 08 |  |
| Fireball | 82 | 08 |  |
| Flame Arrow | 83 | 08 |  |
| Floating Disk | 83 | 08 |  |
| Fly | 83 | 08 |  |
| Fool’s Gold | 83 | 08 |  |
| Forceful Hand | 83 | 08 |  |
| Forget | 84 | 08 |  |
| Freezing Sphere | 84 | 09 |  |
| Friends | 84 | 09 |  |
| Fumble | 84 | 09 |  |
| Gate | 84 | 09 |  |
| Geas | 85 | 09 |  |
| Glass-steel | 85 | 09 |  |
| Glasseye | 85 | 09 |  |
| Globe of Invulnerability | 85 | 09 |  |
| Grasping Hand | 85 | 09 |  |
| Guards and Wards | 85 | 09 |  |
| Gust of Wind | 86 | 09 |  |
| Hallucinatory Terrain | 86 | 09 |  |
| Haste | 86 | 09 |  |
| Hold Monster | 86 | 09 |  |
| Hold Person | 87 | 09 |  |
| Hold Portal | 87 | 09 |  |
| Ice Storm | 87 | 09 |  |
| Identify | 87 | 09 |  |
| Imprisonment* | 88 | 09 |  |
| Incendiary Cloud | 88 | 09 |  |
| Infravision | 88 | 09 |  |
| Instant Summons | 88 | 09 |  |
| Interposing Hand | 89 | 09 |  |
| Invisibility | 89 | 09 |  |
| Invisibility, 10 ft Radius | 89 | 09 |  |
| Invisible Stalker | 89 | 09 |  |
| Irresistible Dance | 89 | 09 |  |
| Jump | 89 | 09 |  |
| Knock | 90 | 09 |  |
| Legend Lore | 90 | 09 |  |
| Levitate | 90 | 09 |  |
| Light | 90 | 09 |  |
| Lightning Bolt | 90 | 09 |  |
| Limited Wish | 91 | 09 |  |
| Locate Object | 91 | 09 |  |
| Lower Water* | 91 | 09 |  |
| Mage’s Faithful Hound | 91 | 09 |  |
| Mage’s Sword | 91 | 09 |  |
| Magic Aura | 92 | 09 |  |
| Magic Jar | 92 | 09 |  |
| Magic Missile | 93 | 09 |  |
| Magic Mouth | 93 | 09 |  |
| Mass Charm | 93 | 09 |  |
| Mass Invisibility | 93 | 09 |  |
| Massmorph | 93 | 09 |  |
| Maze | 93 | 09 |  |
| Mending | 94 | 09 |  |
| Message | 94 | 09 |  |
| Meteor Swarm | 94 | 09 |  |
| Mind Blank | 94 | 09 |  |
| Minor Globe of Invulnerability | 94 | 09 |  |
| Mirror Image | 94 | 09 |  |
| Mnemonic Enhancement | 95 | 09 |  |
| Monster Summoning I | 95 | 09 |  |
| Monster Summoning II | 95 | 09 |  |
| Monster Summoning III | 95 | 09 |  |
| Monster Summoning IV | 96 | 09 |  |
| Monster Summoning V | 96 | 09 |  |
| Monster Summoning VI | 96 | 09 |  |
| Monster Summoning VII | 96 | 09 |  |
| Move Earth | 97 | 09 |  |
| Part Water | 97 | 09 |  |
| Passwall | 97 | 09 |  |
| Permanency | 97 | 09 |  |
| Phantasmal Force | 97 | 10 |  |
| Phase Door | 98 | 10 |  |
| Plant Growth | 98 | 10 |  |
| Polymorph Object | 98 | 10 |  |
| Polymorph Other | 98 | 10 |  |
| Polymorph Self | 99 | 10 |  |
| Power Word, Blind | 99 | 10 |  |
| Power Word, Kill | 99 | 10 |  |
| Power Word, Stun | 99 | 10 |  |
| Prismatic Sphere | 100 | 10 |  |
| Project Image | 100 | 10 |  |
| Pro. From Evil* | 100 | 10 |  |
| Pro. From Evil 10 ft Radius* | 100 | 10 |  |
| Pro. From Normal Missiles | 100 | 10 |  |
| Push | 101 | 10 |  |
| Pyrotechnics | 101 | 10 |  |
| Ray of Enfeeblement | 101 | 10 |  |
| Read Magic* | 101 | 10 |  |
| Remove Curse* | 101 | 10 |  |
| Reincarnation | 102 | 10 |  |
| Repulsion | 102 | 10 |  |
| Reverse Gravity | 102 | 10 |  |
| Rope Trick | 102 | 10 |  |
| Scare | 102 | 10 |  |
| Secret Chest | 103 | 10 |  |
| Shape Change | 103 | 10 |  |
| Shatter | 103 | 10 |  |
| Shield | 103 | 10 |  |
| Shocking Grasp | 103 | 10 |  |
| Simulacrum | 104 | 10 |  |
| Sleep | 104 | 10 |  |
| Slow | 104 | 10 |  |
| Spell Immunity | 104 | 10 |  |
| Spider Climb | 104 | 10 |  |
| Spirit-Rack | 105 | 10 |  |
| Statue | 105 | 10 |  |
| Stinking Cloud | 105 | 10 |  |
| Stone Shape | 105 | 10 |  |
| Stone to Flesh* | 106 | 10 |  |
| Strength | 106 | 10 |  |
| Suggestion | 106 | 10 |  |
| Symbol | 106 | 10 |  |
| Telekinesis | 107 | 10 |  |
| Teleport | 107 | 10 |  |
| Temporal Stasis* | 107 | 10 |  |
| Time Stop | 107 | 10 |  |
| Tiny Hut | 108 | 10 |  |
| Tongues* | 108 | 10 |  |
| Transformation | 108 | 10 |  |
| Transmute Rock to Mud | 108 | 10 |  |
| Trap the Soul | 108 | 10 |  |
| Unseen Servant | 109 | 10 |  |
| Vanish | 109 | 10 |  |
| Ventriloquism | 109 | 10 |  |
| Wall of Fire | 109 | 10 |  |
| Wall of Force | 109 | 10 |  |
| Wall of Ice | 110 | 10 |  |
| Wall of Iron | 110 | 10 |  |
| Wall of Stone | 110 | 10 |  |
| Water Breathing* | 110 | 10 |  |
| Web | 110 | 10 |  |
| Wish | 111 | 10 |  |
| Wizard Eye | 111 | 10 |  |
| Wizard Lock | 111 | 10 |  |
| Write | 111 | 10 |  |

### Illusionist

| Entry | Page | File | Note |
|---|---|---|---|
| Alter Reality | 112 | 11 |  |
| Arcane Spells, Level 1 | 112 | 11 |  |
| Astral Spell | 112 | 11 |  |
| Audible Glamour | 112 | 11 |  |
| Blindness | 112 | 11 |  |
| Blur | 112 | 11 |  |
| Change Self | 112 | 11 |  |
| Chaos | 113 | 11 |  |
| Colour Spray | 113 | 11 |  |
| Confusion | 113 | 11 |  |
| Conjure Animals | 113 | 11 |  |
| Continual Darkness | 113 | 11 |  |
| Continual Light | 113 | 11 |  |
| Dancing Lights | 114 | 11 |  |
| Darkness | 114 | 11 |  |
| Deafness | 114 | 11 |  |
| Demi-Shadow Magic | 114 | 11 |  |
| Demi-Shadow Monsters | 114 | 11 |  |
| Detect Illusion | 114 | 11 |  |
| Detect Invisibility | 114 | 11 |  |
| Detect Magic | 114 | 11 |  |
| Dispel Exhaustion | 115 | 11 |  |
| Dispel Illusion | 115 | 11 |  |
| Emotion | 115 | 11 |  |
| Fear | 115 | 11 |  |
| Fog Cloud | 115 | 11 |  |
| Gaze Reflection | 115 | 11 |  |
| Hallucinatory Terrain | 115 | 11 |  |
| Hypnotic Pattern | 116 | 11 |  |
| Hypnotism | 116 | 11 |  |
| Illusory Script | 116 | 11 |  |
| Improved Invisibility | 116 | 11 |  |
| Improved Phantasmal Force | 116 | 11 |  |
| Invisibility | 116 | 11 |  |
| Invisibility 10 ft Radius | 117 | 11 |  |
| Light | 117 | 11 |  |
| Magic Mouth | 117 | 11 |  |
| Major Creation | 117 | 11 |  |
| Mass Suggestion | 117 | 11 |  |
| Massmorph | 117 | 11 |  |
| Maze | 117 | 11 |  |
| Minor Creation | 117 | 11 |  |
| Mirror Image | 118 | 11 |  |
| Misdirection | 118 | 11 |  |
| Non-Detection | 118 | 11 |  |
| Paralysation | 118 | 11 |  |
| Permanent Illusion | 118 | 11 |  |
| Phantasmal Force | 118 | 11 |  |
| Phantasmal Killer | 118 | 11 |  |
| Prismatic Spray | 119 | 11 |  |
| Prismatic Wall | 119 | 11 |  |
| Programmed Illusion | 119 | 11 |  |
| Project Image | 119 | 11 |  |
| Rope Trick | 119 | 11 |  |
| Shades | 119 | 11 |  |
| Shadow Door | 120 | 11 |  |
| Shadow Magic | 120 | 11 |  |
| Shadow Monsters | 120 | 11 |  |
| Spectral Force | 120 | 11 |  |
| Suggestion | 121 | 11 |  |
| Summon Shadow | 121 | 11 |  |
| True Sight | 121 | 11 |  |
| Veil | 121 | 11 |  |
| Ventriloquism | 121 | 11 |  |
| Vision | 121 | 11 |  |
| Wall of Fog | 121 | 11 |  |

## Monsters

### Men

| Entry | Page | File | Note |
|---|---|---|---|
| Bandit (Brigand) | 194 | 17a |  |
| Berserker | 194 | 17a |  |
| Buccaneer (Pirate) | 194 | 17a |  |
| Dervish (Nomad) | 195 | 17a |  |
| Pilgrim | 196 | 17a |  |
| Merchant | 196 | 17a |  |

### Demi-Humans

| Entry | Page | File | Note |
|---|---|---|---|
| Dwarf | 197 | 17a |  |
| Elf | 197 | 17a |  |
| Gnome | 198 | 17a |  |
| Halfling | 198 | 17a |  |

### Humanoids

| Entry | Page | File | Note |
|---|---|---|---|
| Batrachian | 199 | 17b |  |
| Bugbear | 200 | 17b |  |
| Caveman (Tribesman) | 200 | 17b |  |
| Gnoll | 200 | 17b |  |
| Goblin | 201 | 17b |  |
| Grimlock | 202 | 17b |  |
| Hobgoblin | 203 | 17b |  |
| Kobold | 203 | 17b |  |
| Lizard Man | 203 | 17b |  |
| Orc | 204 | 17b |  |
| Troglodyte | 204 | 17b |  |

### Giants

| Entry | Page | File | Note |
|---|---|---|---|
| Cyclops | 205 | 17b |  |
| Giant, Cloud | 205 | 17b |  |
| Giant, Fire | 206 | 17b |  |
| Giant, Frost | 206 | 17b |  |
| Giant, Hill | 207 | 17b |  |
| Giant, Stone | 207 | 17b |  |
| Giant, Storm | 207 | 17b |  |
| Ettin | 208 | 17b |  |
| Ogre | 208 | 17b |  |
| Troll | 209 | 17b |  |
| Troll, Giant | 209 | 17b |  |
| Troll, Giant Two-Headed | 210 | 17b |  |
| Troll, Ice | 210 | 17b |  |
| Troll, Spectral | 211 | 18 |  |

### Dragons

| Entry | Page | File | Note |
|---|---|---|---|
| Dragon, Black | 211 | 18 |  |
| Dragon, Blue | 212 | 18 |  |
| Dragon, Brass | 212 | 18 |  |
| Dragon, Bronze | 213 | 18 |  |
| Dragon, Copper | 214 | 18 |  |
| Dragon, Gold | 214 | 18 |  |
| Dragon, Green | 214 | 18 |  |
| Dragon, Red | 215 | 18 |  |
| Dragon, Silver | 216 | 18 |  |
| Dragon, White | 216 | 18 |  |

### Demons

| Entry | Page | File | Note |
|---|---|---|---|
| Babau | 217 | 18 |  |
| Class A Demon | 218 | 18 |  |
| Class B Demon | 218 | 18 |  |
| Class C Demon | 219 | 18 |  |
| Class D Demon | 219 | 18 |  |
| Class E Demon | 220 | 18 |  |
| Class F Demon | 221 | 18 |  |
| Demonette | 221 | 18 |  |
| Demoniac | 222 | 18 |  |
| Dretch | 222 | 18 |  |
| Ekivu | 222 | 18 |  |
| Kullule | 223 | 18 |  |
| Quasit | 223 | 18 |  |
| Shub | 224 | 18 |  |
| Succubus | 224 | 18 |  |
| Uduk | 225 | 19 |  |

### Devils

| Entry | Page | File | Note |
|---|---|---|---|
| Assagim | 226 | 19 |  |
| Barbed Devil | 226 | 19 |  |
| Bearded Devil | 227 | 19 |  |
| Bone Devil | 227 | 19 |  |
| Devilcat | 228 | 19 |  |
| Erinyes | 228 | 19 |  |
| Horned Devil | 229 | 19 |  |
| Ice Devil | 229 | 19 |  |
| Imp | 229 | 19 |  |
| Lemure | 230 | 19 |  |
| Scaly Devil | 230 | 19 |  |
| Shaitan | 231 | 19 |  |
| Spiked Devil | 231 | 19 |  |
| Pit Fiend | 232 | 19 |  |
| Soul Worm | 232 | 19 |  |

### Dinosaurs

| Entry | Page | File | Note |
|---|---|---|---|
| Tyrannosaurids/Allosaurids | 233 | 19 |  |
| Hadrosaurids | 233 | 19 |  |
| Sauropods | 234 | 19 |  |
| Ceratopsians | 235 | 19 |  |
| Other Dinosaurs I | 235 | 19 |  |
| Other Dinosaurs II | 236 | 19 |  |
| Marine Dinosaurs | 236 | 19 |  |
| Flying Dinosaurs | 237 | 19 |  |

### Golems

| Entry | Page | File | Note |
|---|---|---|---|
| Flesh | 237 | 19 |  |
| Stone | 237 | 19 |  |
| Iron | 237 | 19 |  |
| Clay | 237 | 19 |  |

### Lycanthropes

| Entry | Page | File | Note |
|---|---|---|---|
| Werebear | 238 | 19 |  |
| Wereboar | 238 | 19 |  |
| Wererat | 238 | 19 |  |
| Weretiger | 238 | 19 |  |
| Werewold | 238 | 19 |  |

### Sylvan Or Faerie Creatures

| Entry | Page | File | Note |
|---|---|---|---|
| Brownie | 240 | 20 |  |
| Centaur | 240 | 20 |  |
| Dryad | 240 | 20 |  |
| Faun (Satyr) | 241 | 20 |  |
| Leprechaun | 241 | 20 |  |
| Nixie | 241 | 20 |  |
| Nymph | 242 | 20 |  |
| Pixie | 243 | 20 |  |
| Quickling | 243 | 20 |  |
| Sprite | 244 | 20 |  |
| Sylph | 244 | 20 |  |
| Treant | 244 | 20 |  |
| Tree, Animated | 244 | 20 |  |
| Unicorn | 245 | 20 |  |

### Undead

| Entry | Page | File | Note |
|---|---|---|---|
| Banshee (Groaning Spirit) | 245 | 20 |  |
| Coffer Corpse | 245 | 20 |  |
| Ghast | 246 | 20 |  |
| Ghost | 246 | 20 |  |
| Ghoul | 247 | 20 |  |
| Lich | 247 | 20 |  |
| Mummy | 248 | 20 |  |
| Poltergeist | 248 | 20 |  |
| Shadow | 249 | 20 |  |
| Skeleton | 249 | 20 |  |
| Spectre | 250 | 20 |  |
| Vampire | 250 | 20 |  |
| Wight | 251 | 20 |  |
| Wraith | 251 | 20 |  |
| Zombie | 251 | 20 |  |
| Zombie, Juju | 252 | 20 |  |

### Animals

| Entry | Page | File | Note |
|---|---|---|---|
| Ape | 252 | 21 |  |
| Axe Beak (Phorusrhacid) | 253 | 21 |  |
| Baboon | 253 | 21 |  |
| Badger | 253 | 21 |  |
| Bat | 253 | 21 |  |
| Bat, Mobat | 254 | 21 |  |
| Barracuda | 254 | 21 |  |
| Bear, Lesser | 254 | 21 |  |
| Bear, Greater | 254 | 21 |  |
| Bird | 255 | 21 |  |
| Boar | 255 | 21 |  |
| Boar, Warthog | 255 | 21 |  |
| Camel | 256 | 21 |  |
| Cat | 256 | 21 |  |
| Cattle | 256 | 21 |  |
| Crocodile | 257 | 21 |  |
| Crustacean, Giant | 257 | 21 |  |
| Dog | 258 | 21 |  |
| Eel, Giant | 258 | 21 |  |
| Elephant | 258 | 21 |  |
| Fish, Giant | 259 | 21 |  |
| Frog, Giant | 260 | 21 |  |
| Horse | 260 | 21 |  |
| Hippopotamus | 261 | 21 |  |
| Hyena | 261 | 21 |  |
| Indricotherium | 261 | 21 |  |
| Jackal | 262 | 21 |  |
| Lion | 262 | 21 |  |
| Mule | 263 | 21 |  |
| Portuguese Man O’ War, Giant | 263 | 21 |  |
| Rat | 263 | 21 |  |
| Rhinoceros | 264 | 21 |  |
| Shark | 264 | 21 |  |
| Squid, Giant | 264 | 21 |  |
| Tiger | 265 | 21 |  |
| Toad | 265 | 21 |  |
| Turtle | 265 | 21 |  |
| Walrus | 266 | 21 |  |
| Weasel | 266 | 21 |  |
| Whale | 266 | 21 |  |
| Wolf | 267 | 21 |  |
| Wolverine | 267 | 21 |  |
| Worg | 268 | 21 |  |

### Other Creatures

| Entry | Page | File | Note |
|---|---|---|---|
| Achaierai | 268 | 22a |  |
| Aerial Servant | 268 | 22a |  |
| Afreet | 269 | 22a |  |
| Al-Mi’raj | 269 | 22a |  |
| Amber Creeping Vine | 269 | 22a |  |
| Ankheg | 270 | 22a |  |
| Annis | 270 | 22a |  |
| Ant, Giant | 271 | 22a |  |
| Aurumvorax | 271 | 22a |  |
| Babbler | 271 | 22a |  |
| Barghest | 272 | 22a |  |
| Basilisk | 272 | 22a |  |
| Bee, Giant | 272 | 22a |  |
| Beetle, Giant | 273 | 22a |  |
| Behir | 274 | 22a |  |
| Blindheim | 274 | 22a |  |
| Blink Dog | 274 | 22a |  |
| Bulette | 275 | 22a |  |
| Carbuncle | 275 | 22a |  |
| Carcass Creeper | 276 | 22a |  |
| Caryatid Column | 276 | 22a |  |
| Caterwaul | 276 | 22a |  |
| Centipede | 277 | 22b |  |
| Chimæra | 277 | 22b |  |
| Cockatrice | 277 | 22b |  |
| Coeurl | 278 | 22b |  |
| Couatl | 278 | 22b |  |
| Crabman | 278 | 22b |  |
| Crypt Thing | 279 | 22b |  |
| Dakon | 279 | 22b |  |
| Dark Creeper | 279 | 22b |  |
| Disenchanter | 281 | 22b |  |
| Doppelgänger | 281 | 22b |  |
| Dracolisk | 281 | 22b |  |
| Dragon Turtle | 282 | 22b |  |
| Elemental | 282 | 22b |  |
| Ettercap | 284 | 22b |  |
| Executioner’s Hood | 284 | 22b |  |
| Eye of the Deep | 284 | 22b |  |
| Fly, Giant | 284 | 22b |  |
| Fungi, Violet | 285 | 22b |  |
| Gargoyle | 285 | 22b |  |
| Gelatinous Cube | 285 | 23a |  |
| Genie | 286 | 23a |  |
| Gorgon | 286 | 23a |  |
| Grey Ooze | 287 | 23a |  |
| Griffon | 287 | 23a |  |
| Harpy | 287 | 23a |  |
| Hell Hound | 288 | 23a |  |
| Hippogriff | 288 | 23a |  |
| Homonculus | 288 | 23a |  |
| Hydra | 289 | 23a |  |
| Invisible Stalker | 289 | 23a |  |
| Jackalwere | 290 | 23a |  |
| Kraken | 290 | 23a |  |
| Lamia | 291 | 23a |  |
| Lammasu | 291 | 23a |  |
| Leech, Giant | 291 | 23a |  |
| Lizard, Giant | 292 | 23a |  |
| Locathah | 293 | 23a |  |
| Lurker Above | 293 | 23a |  |
| Manticore | 293 | 23a |  |
| Medusa | 294 | 23a |  |
| Mephit | 294 | 23a |  |
| Merman | 295 | 23a |  |
| Minotaur | 296 | 23b |  |
| Mongrelman | 296 | 23b |  |
| Mould | 297 | 23b |  |
| Naga | 297 | 23b |  |
| Necrophidius | 298 | 23b |  |
| Nereid | 299 | 23b |  |
| Night Hag | 299 | 23b |  |
| Nightmare | 300 | 23b |  |
| Nilbog | 300 | 23b |  |
| Owlbear | 300 | 23b |  |
| Otyugh | 301 | 23b |  |
| Pegasus | 301 | 23b |  |
| Phantom | 302 | 23b |  |
| Phoenix | 302 | 23b |  |
| Piercer | 303 | 23b |  |
| Pseudo-Dragon | 303 | 23b |  |
| Purple Worm | 304 | 23b |  |
| Rakshasa | 304 | 23b |  |
| Remorhaz | 304 | 23b |  |
| Roc | 305 | 24 |  |
| Roper | 305 | 24 |  |
| Rot Grub | 306 | 24 |  |
| Rust Monster | 307 | 24 |  |
| Sahuagin | 307 | 24 |  |
| Scorpion | 308 | 24 |  |
| Sea Hag | 308 | 24 |  |
| Sea Serpent | 309 | 24 |  |
| Shambling Mound | 309 | 24 |  |
| Shedu | 309 | 24 |  |
| Shrieker | 310 | 24 |  |
| Skeleton Warrior | 310 | 24 |  |
| Slithering Tracker | 311 | 24 |  |
| Slime, Green | 311 | 24 |  |
| Slug, Giant | 311 | 24 |  |
| Snake, Giant | 312 | 24 |  |
| Sphinx | 312 | 24 |  |
| Sphinx, Andro- | 312 | 24 |  |
| Sphinx, Crio- | 313 | 24 |  |
| Sphinx, Gyno- | 313 | 24 |  |
| Sphinx, Hieraco- | 314 | 24 |  |
| Spider, Giant | 314 | 24 |  |
| Spider, Huge | 314 | 24 |  |
| Spider, Large | 314 | 24 |  |
| Spider, Phase | 315 | 24 |  |
| Spider, Giant Water | 315 | 24 |  |
| Squealer | 315 | 24 |  |
| Stirge | 316 | 24 |  |
| Stunjelly | 316 | 24 |  |
| Tick, Giant | 316 | 24 |  |
| Titan | 316 | 24 |  |
| Trapper | 317 | 24 |  |
| Triton | 317 | 24 |  |
| Vilstrak | 318 | 24 |  |
| Volt | 318 | 24 |  |
| Vulchling | 318 | 24 |  |
| Wasp, Giant | 319 | 24 |  |
| Will-O-the-Wisp | 319 | 24 |  |
| Wyvern | 319 | 24 |  |
| Xorn | 319 | 24 |  |
| Yeti | 320 | 24 |  |
| Dread Wraith | 372 | 29b | embedded in the Deck of Many Things entry, not a standalone heading; printed out of sequence in the book's own List of Monsters (after Yeti), pointing into the Artifacts page range — reproduced as printed, see the leave-alone list in 05 errata.md |

## Magic Items

### Potions

| Entry | Page | File | Note |
|---|---|---|---|
| Animal Control | 329 | 25 |  |
| Clairaudience | 329 | 25 |  |
| Clairvoyance | 329 | 25 |  |
| Climbing | 329 | 25 |  |
| Delusion | 329 | 25 |  |
| Diminution | 329 | 25 |  |
| Dragon Control | 329 | 25 |  |
| ESP | 330 | 25 |  |
| Extra-Healing | 330 | 25 |  |
| Fire Resistance | 330 | 25 |  |
| Flying | 330 | 25 |  |
| Gaseous Form | 330 | 25 |  |
| Giant Control | 330 | 25 |  |
| Giant Strength | 330 | 25 |  |
| Growth | 330 | 25 |  |
| Healing | 330 | 25 |  |
| Heroism | 330 | 25 |  |
| Human Control | 330 | 25 |  |
| Invisibility | 331 | 25 |  |
| Invulnerability | 331 | 25 |  |
| Levitation | 331 | 25 |  |
| Longevity | 331 | 25 |  |
| Oil of Ætherealness | 331 | 25 |  |
| Oil of Slipperiness | 331 | 25 |  |
| Philtre of Love | 331 | 25 |  |
| Philtre of Persuasiveness | 331 | 25 |  |
| Plant Control | 331 | 25 |  |
| Polymorph | 331 | 25 |  |
| Speed | 331 | 25 |  |
| Super-Heroism | 331 | 25 |  |
| Sweet Water | 332 | 25 |  |
| Treasure Finding | 332 | 25 |  |
| Undead Control | 332 | 25 |  |
| Water Breathing | 332 | 25 |  |

### Scrolls

| Entry | Page | File | Note |
|---|---|---|---|
| Ward of Demons | 333 | 25 |  |
| Ward of Devils | 333 | 25 |  |
| Ward of Elementals | 333 | 25 |  |
| Ward of Lycanthropes | 333 | 25 |  |
| Ward of Magic | 333 | 25 |  |
| Ward of Petrifaction | 333 | 25 |  |
| Ward of Possession | 333 | 25 |  |
| Ward of Undead | 333 | 25 |  |

### Rods, Staves And Wands

| Entry | Page | File | Note |
|---|---|---|---|
| Absorption | 334 | 26 |  |
| Cancellation | 334 | 26 |  |
| Captivation | 334 | 26 |  |
| Lordly Might | 334 | 26 |  |
| Resurrection | 335 | 26 |  |
| Rulership | 335 | 26 |  |
| Striking | 335 | 26 |  |
| Compulsion | 335 | 26 |  |
| Healing | 335 | 26 |  |
| Power | 335 | 26 |  |
| Serpent | 336 | 26 |  |
| Withering | 336 | 26 |  |
| Wizardry | 336 | 26 |  |
| Detecting Magic | 336 | 26 |  |
| Det. Minerals and Metals | 336 | 26 |  |
| Det. Traps and Secret Doors | 337 | 26 |  |
| Enemy Detection | 337 | 26 |  |
| Fear | 337 | 26 |  |
| Fire | 337 | 26 |  |
| Ice | 337 | 26 |  |
| Light | 337 | 26 |  |
| Illusion | 337 | 26 |  |
| Lightning | 337 | 26 |  |
| Magic Missiles | 337 | 26 |  |
| Negation | 337 | 26 |  |
| Paralysation | 338 | 26 |  |
| Polymorphing | 338 | 26 |  |
| Summoning | 338 | 26 |  |
| Wonder | 338 | 26 |  |

### Magic Armour And Shields

| Entry | Page | File | Note |
|---|---|---|---|
| Plate Mail of Æthereality | 338 | 26 |  |
| Large Shield +1, Missile Deflector | 339 | 26 | printed as "L Shield" in the audited 01 lists.md roster (leave-alone list) but transcribed in file 26 as "Large Shield" per that file's own independent raster/bbox verification — unresolved owner-decision conflict, see loose ends and backlog |

### Magic Swords

| Entry | Page | File | Note |
|---|---|---|---|
| Bleeding Sword | 339 | 26 |  |
| Dancing Sword | 339 | 26 |  |
| Defender | 339 | 26 |  |
| Dragonbane | 339 | 26 |  |
| Flaming Blade | 339 | 26 |  |
| Frost Brand | 339 | 26 |  |
| Giantbane | 340 | 26 |  |
| Holy Sword | 340 | 26 |  |
| Keenblade | 340 | 26 |  |
| Luck Blade | 340 | 26 |  |
| Magebane | 340 | 26 |  |
| Nine Lives Stealer | 340 | 26 |  |
| Trollbane | 340 | 26 |  |
| Vampire Blade | 340 | 26 |  |
| Vorpal Blade | 340 | 26 |  |
| Werebane | 340 | 26 |  |
| Wyrmbane | 340 | 26 |  |

### Miscellaneous Weapons

| Entry | Page | File | Note |
|---|---|---|---|
| Arrow of Slaying | 343 | 26 |  |
| Axe of Hurling | 343 | 26 |  |
| Crossbow of Accuracy | 343 | 26 |  |
| Crossbow of Range | 343 | 26 |  |
| Crossbow of Speed | 343 | 26 |  |
| Dagger of Venom | 343 | 26 |  |
| Hammer of the Dwarfs | 344 | 26 |  |
| Holy Mace | 344 | 26 |  |
| Sling of the Halfling | 344 | 26 |  |
| Trident/Fork | 344 | 26 |  |

### Miscellaneous Magic

| Entry | Page | File | Note |
|---|---|---|---|
| Afreeti Bottle | 344 | 27 |  |
| Ahmek’s Copious Coin Purse | 344 | 27 |  |
| Alchemy Jug | 344 | 27 |  |
| Amulet of Health | 344 | 27 |  |
| Amulet of Mighty Fists | 344 | 27 |  |
| Amulet of Natural Armour | 344 | 27 |  |
| Amulet of Life Protection | 344 | 27 |  |
| Amulet of the Planes | 345 | 27 |  |
| Amulet of Proof Against Detection or Location | 345 | 27 |  |
| Apparatus of the Lobster | 345 | 27 |  |
| Arrow of Direction | 345 | 27 |  |
| Bag of Holding | 345 | 27 |  |
| Bag of Tricks | 345 | 27 |  |
| Bead of Force | 345 | 27 |  |
| Belt of Dwarfkind | 346 | 27 |  |
| Belt of Giant Strength | 346 | 27 |  |
| Blemish Blotter | 346 | 27 |  |
| Blessed Book | 346 | 27 |  |
| Boat, Folding | 346 | 27 |  |
| Boots of Elvenkind | 346 | 27 |  |
| Boots of Levitation | 346 | 27 |  |
| Boots of Speed | 346 | 27 |  |
| Boots of Striding/Springing | 346 | 27 |  |
| Boots of Teleportation | 346 | 27 |  |
| Boots of the Winterlands | 346 | 27 |  |
| Boots, Winged | 346 | 27 |  |
| Bottle of Air | 346 | 27 |  |
| Bowl Commanding Water Elementals | 346 | 27 |  |
| Bracelet of Friends | 347 | 27 |  |
| Bracers of Archery, Greater | 347 | 27 |  |
| Bracers of Archery, Lesser | 347 | 27 |  |
| Bracers of Armour | 347 | 27 |  |
| Brazier of Commanding Fire Elementals | 347 | 27 |  |
| Brooch of Instigation | 347 | 27 |  |
| Brooch of Shielding | 347 | 27 |  |
| Broom of Flying | 347 | 27 |  |
| Candle of Invocation | 347 | 27 |  |
| Candle of Truth | 347 | 27 |  |
| Cape of the Mountebank | 347 | 27 |  |
| Carpet of Flying | 347 | 27 |  |
| Censer of Controlling Air Elementals | 348 | 27 |  |
| Chime of Interruption | 348 | 27 |  |
| Chime of Opening | 348 | 27 |  |
| Circlet of Blasting, Major | 348 | 27 |  |
| Circlet of Blasting, Minor | 348 | 27 |  |
| Circlet of Persuasion | 348 | 27 |  |
| Cloak of Arachnida | 348 | 27 |  |
| Cloak of the Bat | 348 | 27 |  |
| Cloak of Charisma | 348 | 27 |  |
| Cloak of Displacement, Major | 348 | 27 |  |
| Cloak of Displacement, Minor | 348 | 27 |  |
| Cloak of Elvenkind | 348 | 27 |  |
| Cloak of Ætherealness | 348 | 27 |  |
| Cloak of the Manta Ray | 348 | 27 |  |
| Cloak of Resistance | 348 | 27 |  |
| Crystal Ball | 349 | 27 |  |
| Cube of Force | 349 | 27 |  |
| Cube of Frost Resistance | 349 | 27 |  |
| Cubic Gate | 349 | 27 |  |
| Dark Skull | 349 | 27 |  |
| Decanter of Endless Water | 349 | 27 |  |
| Deck of Illusions | 350 | 27 |  |
| Dimensional Shackles | 350 | 27 |  |
| Drums of Panic | 350 | 27 |  |
| Dust of Appearance | 350 | 27 |  |
| Dust of Disappearance | 350 | 27 |  |
| Dust of Dryness | 351 | 27 |  |
| Dust of Illusion | 351 | 27 |  |
| Dust of Tracelessness | 351 | 27 |  |
| Efficient Quiver | 351 | 27 |  |
| Elemental Gem | 351 | 27 |  |
| Elixir of Fire Breath | 351 | 27 |  |
| Elixir of Hiding | 351 | 27 |  |
| Elixir of Swimming | 351 | 27 |  |
| Elixir of Truth | 351 | 27 |  |
| Elixir of Vision | 351 | 27 |  |
| Eversmoking Bottle | 351 | 27 |  |
| Eyes of Charming | 351 | 27 |  |
| Eyes of Doom | 351 | 27 |  |
| Eyes of the Eagle | 352 | 27 |  |
| Eyes of Petrifaction | 352 | 27 |  |
| Feather Token | 352 | 27 |  |
| Figurines of Wondrous Power | 352 | 27 |  |
| Gauntlets of Ogre Power | 353 | 27 |  |
| Gauntlet of Rust | 353 | 27 |  |
| Gem of Brightness | 353 | 27 |  |
| Gem of Seeing | 353 | 27 |  |
| Gloves of Arrow Snaring | 353 | 27 |  |
| Gloves of Dexterity | 353 | 27 |  |
| Glove of Storing | 353 | 27 |  |
| Gloves of Swimming/Climbing | 353 | 27 |  |
| Goggles of Minute Seeing | 353 | 27 |  |
| Goggles of Night | 353 | 28 |  |
| Golem Manual | 353 | 28 |  |
| Handy Haversack | 353 | 28 |  |
| Harp of Charming | 353 | 28 |  |
| Hat of Disguise | 353 | 28 |  |
| Headband of Intellect | 353 | 28 | not in the book's own front-matter List of Magic Items (PDF 10) — genuinely printed and described in file 28's body text; front-matter omission found in batch 14, file 01 (01 lists.md) is not at fault, see loose ends and backlog |
| Helm of Brilliance | 353 | 28 |  |
| Helm of Comprehend Languages | 354 | 28 |  |
| Helm of Telepathy | 354 | 28 |  |
| Helm of Teleportation | 354 | 28 |  |
| Helm of Underwater Action | 354 | 28 |  |
| Horn of Blasting | 354 | 28 |  |
| Horn of Blasting, Greater | 354 | 28 |  |
| Horn of Fog | 354 | 28 |  |
| Horn of Goodness/Evil | 354 | 28 |  |
| Horn of the Tritons | 354 | 28 |  |
| Horn of Valhalla | 355 | 28 |  |
| Horseshoes of Speed | 355 | 28 |  |
| Horseshoes of the Zephyr | 355 | 28 |  |
| Incense of Meditation | 355 | 28 |  |
| Instant Fortress | 355 | 28 |  |
| Ioun Stones | 355 | 28 |  |
| Iron Bands of Binding | 355 | 28 |  |
| Iron Flask | 355 | 28 |  |
| Javelin of the Raptor | 356 | 28 |  |
| Lantern of Revealing | 356 | 28 |  |
| Lyre of Building | 356 | 28 |  |
| Mantle of Faith | 356 | 28 |  |
| Mantle of Magic Resistance | 356 | 28 |  |
| Manual of Bodily Health | 356 | 28 |  |
| Manual of Gainful Exercise | 356 | 28 |  |
| Manual of Quickness of Action | 356 | 28 |  |
| Marvellous Pigments | 356 | 28 |  |
| Mask of the Skull | 356 | 28 |  |
| Mattock of the Titans | 356 | 28 |  |
| Maul of the Titans | 356 | 28 |  |
| Medallion of Thoughts | 356 | 28 |  |
| Mirror of Life Trapping | 356 | 28 |  |
| Mirror of Mental Prowess | 357 | 28 |  |
| Mirror of Opposition | 357 | 28 |  |
| Necklace of Adaptation | 357 | 28 |  |
| Necklace of Fireballs | 357 | 28 |  |
| Oil of Famishing | 357 | 28 |  |
| Orb of Storms | 357 | 28 |  |
| Pearl of Power | 358 | 28 |  |
| Pearl of the Sirines | 358 | 28 |  |
| Periapt of Health | 358 | 28 |  |
| Periapt of Proof Against Poison | 358 | 28 |  |
| Periapt of Wisdom | 358 | 28 |  |
| Periapt of Wound Closure | 358 | 28 |  |
| Phylactery of Faithfulness | 358 | 28 |  |
| Phylactery of Undead Turning | 358 | 28 |  |
| Pipes of Haunting | 358 | 28 |  |
| Pipes of Pain | 358 | 28 |  |
| Pipes of the Sewers | 358 | 28 |  |
| Pipes of Sounding | 358 | 28 |  |
| Plentiful Vessel | 358 | 28 |  |
| Portable Hole | 358 | 28 | not in the book's own front-matter List of Magic Items (PDF 10) — genuinely printed and described in file 28's body text; front-matter omission found in batch 14, file 01 (01 lists.md) is not at fault, see loose ends and backlog |
| Restorative Ointment | 358 | 28 |  |
| Ring Gates | 358 | 28 |  |
| Robe of the Archmagi | 359 | 28 |  |
| Robe of Blending | 359 | 28 |  |
| Robe of Bones | 359 | 28 |  |
| Robe of Eyes | 359 | 28 |  |
| Robe of Scintillating Colours | 359 | 28 |  |
| Robe of Stars | 359 | 28 |  |
| Robe of Useful Items | 359 | 28 |  |
| Rope of Climbing | 360 | 28 |  |
| Rope of Entanglement | 360 | 28 |  |
| Sagacious Volume | 360 | 28 |  |
| Scabbard of Keen Edges | 360 | 28 |  |
| Scarab of Golem Bane | 360 | 28 |  |
| Scarab of Protection | 360 | 28 |  |
| Shrouds of Disintegration | 360 | 28 |  |
| Silversheen | 360 | 28 |  |
| Slippers of Spider Climbing | 360 | 28 |  |
| Sovereign Glue | 360 | 28 |  |
| Stone of Alarm | 360 | 28 |  |
| Stone of Controlling Earth | 360 | 28 |  |
| Stone of Good Luck | 360 | 28 |  |
| Stone Horse | 361 | 28 |  |
| Stone Salve | 361 | 28 |  |
| Strand of Prayer Beads | 361 | 28 |  |
| Sustaining Spoon | 361 | 28 |  |
| Thunder Spear | 361 | 28 |  |
| Tome of Clear Thought | 361 | 28 |  |
| Tome of Leadership/Influence | 361 | 28 |  |
| Tome of Understanding | 361 | 28 |  |
| Unguent of Timelessness | 361 | 28 |  |
| Universal Solvent | 361 | 28 |  |
| Vest of Escape | 361 | 28 |  |
| Vestment, Druid’s | 361 | 28 |  |
| Well of Many Worlds | 361 | 28 |  |
| Wind Fan | 362 | 28 |  |
| Wings of Flying | 362 | 28 |  |

### Rings

| Entry | Page | File | Note |
|---|---|---|---|
| Ring of Charisma | 362 | 29a |  |
| Ring of Feather Falling | 362 | 29a |  |
| Ring of Fire Resistance | 362 | 29a |  |
| Ring of Free Action | 362 | 29a |  |
| Ring of Genie Summoning | 362 | 29a |  |
| Ring of Invisibility | 362 | 29a |  |
| Ring of Protection | 362 | 29a |  |
| Ring of Regeneration | 363 | 29a |  |
| Ring of Spell Storing | 363 | 29a |  |
| Ring of Spell Turning | 363 | 29a | prints as page "63" in the book's own front-matter List of Magic Items — E17, a confirmed printed error; corrected here to the entry's real location between Ring of Spell Storing (363) and Ring of Swimming (364) |
| Ring of Swimming | 364 | 29a |  |
| Ring of Three Wishes | 364 | 29a |  |
| Ring of Warmth | 364 | 29a |  |
| Ring of Water Walking | 364 | 29a |  |
| Ring of Wizardry | 364 | 29a |  |

### Cursed Items

| Entry | Page | File | Note |
|---|---|---|---|
| Amulet of Inescapable Location | 366 | 29a |  |
| Armour of Arrow Attraction | 366 | 29a |  |
| Armour of Rage | 366 | 29a |  |
| Bag of Devouring | 366 | 29a |  |
| Boots of Dancing | 367 | 29a |  |
| Bracers of Defencelessness | 367 | 29a |  |
| Broom of Animated Attack | 367 | 29a |  |
| Cloak of Poisonousness | 367 | 29a |  |
| Crystal Hypnosis Ball | 367 | 29a |  |
| Dust of Sneezing/Choking | 367 | 29a |  |
| Flask of Curses | 367 | 29a |  |
| Gauntlets of Fumbling | 367 | 29a |  |
| Helm of Opposite Alignment | 367 | 29a |  |
| Incense of Obsession | 368 | 29a |  |
| Mace of Blood | 368 | 29a |  |
| Medallion of Thought Projection | 368 | 29a |  |
| Necklace of Strangulation | 368 | 29a |  |
| Net of Snaring | 368 | 29b |  |
| Periapt of Foul Rotting | 368 | 29b |  |
| Plate Mail of Vulnerability | 368 | 29b |  |
| Ring of Clumsiness | 368 | 29b |  |
| Ring of Contrariness | 368 | 29b |  |
| Ring of Weakness | 369 | 29b |  |
| Robe of Powerlessness | 369 | 29b |  |
| Robe of Vermin | 369 | 29b |  |
| Scarab of Death | 369 | 29b |  |
| Shield -1, Missile Attractor | 369 | 29b |  |
| Spear, Cursed Backbiter | 369 | 29b |  |
| Stone of Weight/Loadstone | 369 | 29b |  |
| Sword +1, Cursed | 369 | 29b |  |
| Sword -2, Cursed | 370 | 29b |  |
| Sword of the Berserker +2 | 370 | 29b |  |
| Vacuous Grimoire | 370 | 29b |  |

### Artifacts

| Entry | Page | File | Note |
|---|---|---|---|
| Book of Infinite Spells | 370 | 29b |  |
| Deck of Many Things | 371 | 29b |  |
| Hammer of Thunderbolts | 373 | 29b |  |
| Philosopher’s Stone | 373 | 29b |  |
| Sphere of Annihilation | 373 | 29b |  |
| Talisman of Pure Good | 373 | 29b |  |
| Talisman of the Sphere | 374 | 29b |  |
| Talisman of Reluctant Wishes | 374 | 29b |  |
| Talisman of Pure Evil | 374 | 29b |  |

