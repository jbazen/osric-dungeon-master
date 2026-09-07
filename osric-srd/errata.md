# OSRIC errata — printed errors and known false positives

Two lists. The first is things the book genuinely prints wrong, which
must be **reproduced as printed**. The second is things that look wrong
and are not, which must be **left alone**.

The second list matters more. It is what stops an auditor spending a
session "correcting" the book.

Source: recon parts 1 and 2. Every confirmed item was verified by
rasterising the page and reading it. Not exhaustive — more will surface
during transcription, and this file gets appended to as they do.

---

## Confirmed printed errors

Reproduce exactly as printed. Add an HTML comment immediately after:
`<!-- printed as-is: see errata E4 -->`

| ID | Book p. | PDF p. | Goes in file | What is printed |
|---|---|---|---|---|
| E1 | 398 | 410 | 33 licence | **Ten literal `\t` sequences** in the OGL §15 Tome of Horrors credit lines — e.g. `E. Gary Gygax, Beetle, \t Boring from the Tome of Horrors`. Each stands in for a word in a creature's compound name. **Corrected from eleven.** There are eleven `\t` on the page, but the eleventh is in the Product Identity sentence and is logged separately as E2 — recon double-counted it. Verified by locating every backslash word box on the page (exactly 11) and reading each off a 300 dpi raster. |
| E2 | 398 | 410 | 33 licence | Product Identity sentence, three faults at once: a literal `\t` in `Variable \t Point Rule`; the rule **does not exist** — "Point Rule" appears nowhere else in the book and p.118 is illusionist spells; and `"OSRIC," "OSRIC,"` prints the same term twice where p.ii gives three distinct terms — *OSRIC*, *Osric*, *O.S.R.I.C.* A fourth difference, confirmed by cross-checking the two delivered files: p.398 sets its commas **inside** the closing quotation marks, p.ii sets its comma **outside**. The pages use opposite conventions. |
| E3 | 307 | 319 | 24 monsters other | Stray backslash in a stat block Move row: `120 ft\; 240 ft swimming`. The four adjacent columns print it correctly. |
| E4 | 143 | 155 | 13 hirelings | Henchman Class table: `01-40 Fighter / 41-60 Magic User / 61-80 Cleric / 91-00 Thief`. **81–90 unassigned.** Four rows, no fifth, no note. |
| E5 | 107 | 119 | 10 spells magic user | *Teleport* familiarity table, "Viewed once" row: `01–76 / 77–88 / 89–90 / 99–100`. **91–98 unassigned.** Every other row runs continuous to 100. This table also uses **en-dashes** where most of the book uses hyphens — preserve that. |
| E6 | 327 | 339 | 25 treasure | Table IV Rare Miscellaneous Magic: `03-04 Amulet of Life Protection` then `04-05 Amulet of Mighty Fists`. **04 duplicated.** |
| E7 | 327 | 339 | 25 treasure | Same table: `12-13 Boots of Teleportation` then `13-14 Boots, Winged`. **13 duplicated.** |
| E8 | 125 | 137 | 12 how to play + 30 compiled tables | Item Saving Throw Table, Paper row: **Fireball 25, Fire Magical 21.** Both impossible on d20. No other row exceeds 20. **Reproduced verbatim a SECOND time at book p.387, in file 30's Appendix A reprint of the same table — confirmed on word boxes by audit batch 9. File 30 is correct: it reproduces its page. The "Goes in file" column was corrected to name both files on 2026-09-07.** |
| E9 | 125 | 137 | 12 how to play + 30 compiled tables | Same table: Paper prints `0` under Fall (5ft); Liquid prints `0` under Blow Crushing, Blow Normal and Fall (5ft). Out of the table's own range, and inconsistent with the `—` used elsewhere for not-applicable. **Reproduced verbatim a SECOND time at book p.387, in file 30's Appendix A reprint of the same table. File 30 is correct. "Goes in file" corrected 2026-09-07.** |
| E10 | 13 | 25 | 03 character classes | Druid Saving Throw Table header: **`Breatsh Weapons`**. Correct in the eight other class tables and in the Appendix A duplicate on p.378. |
| E11 | vi | 8 | 01 lists | List of Monsters: **`Werewold`**. |
| E12 | 186 | 198 | 16 urban and wilderness | **`Scorption, Giant`**. |
| E13 | 161 | 173 | 15 dungeons | Random dungeon room table: **`Labouratory`**. Over-applied British spelling, sitting beside correctly-set Kitchen, Library, Temple. |
| E14 | 240 | 252 | 20 monsters sylvan and undead | Brownie entry: *"They speak their own tongue, **halfing**, and can communicate with other…"* Should be halfling. Set correctly everywhere else in the book. |
| E15 | 396 | 408 | 32 index | Index of Tables: **`Artic  179, 180`**. Set correctly as *Arctic* in the body at pp.178, 179, 264, 305, and *subarctic* at pp.259, 265. |
| ~~E16~~ | 388 | 400 | 30 compiled tables | **RETRACTED 2026-09-06 by the owner. E16 was wrong — do not act on it, and do not "restore" the gap it describes.** It read: *“Monster HD / Equivalent Level table: rows for 9+1 to 10, 10+1 to 11 and 11+1 to 12 are absent. The sequence jumps from ‘8+1 to 9 → 10’ to ‘12+1 to 13 → 14’.”* That is true of book p.388 **read in isolation**, but the three “missing” rows are genuinely printed at the **foot of p.387**, in the same table's right-hand column-block, and p.388 then repeats the header and continues both blocks — the column-major, page-spanning convention already documented in `04 geometry and extraction.md` §4. Rasterisation and a `-bbox` check, independently repeated by the file 30 transcriber in batch 16, found the table runs 0 through 21 across the two pages with **no gap at all**. File 30 transcribes it complete and gap-free, and is correct. |
| E17 | viii | 10 | 01 lists | List of Magic Items, RINGS: *Ring of Spell Turning* prints page **63**. Neighbours print 363 and 364. Verified at 600 dpi — the glyphs really are `63`, with no clipped leading digit. That 363 was intended is an inference from the surrounding sequence, not something the page states. Found during transcription, not recon. |
| E18 | 397 | 409 | 33 licence | OSRIC Open License item 7 closes `under the OGL .` — a space before the full stop. The `.` is a separate word box with a gap matching the word gaps on the same line. |
| E19 | 398 | 410 | 33 licence | Trapper credit reads `based on original material **be** E. Gary Gygax`. Every other credit on the page reads "by". |
| E20 | 398 | 410 | 33 licence | Yeti credit reads `Inc author Scott Green based on original material by E. Gary Gygax` — **`Green`** for *Greene*. One instance on p.410; set correctly as "Scott Greene" in all 62 other Tome of Horrors credits on the page. |
| E21 | ix | 11 | 00 front matter | In the `Class;` entry, the opening quotation mark before *class* is set as a **closing** mark (U+201D) where an opening mark belongs. Confirmed by byte inspection, by a 600 dpi comparison against correctly-set pairs on the same page, and by a quote census across the range: 40 opening against 42 closing, an imbalance of exactly one — which also proves there is no second reversed quote in the range. |
| E22 | ix | 11 | 00 front matter | The defined term prints as `Experience bonus:` — a colon and a lower-case *b* — where the other fifteen defined terms on pp.ix–x are all Title Case with a semicolon. **Logged as an inconsistency, not a certain error.** It may be deliberate. Either way it is reproduced as printed and must not be harmonised. |
| E23 | 398 | 410 | 33 licence | OGL clause 1 prints **closing-style quotation marks in opening position** at `(a)”Contributors”`, `(b)”Derivative Material”`, `(d)”Open Game Content”` and `“Use”,”Used”`. Systematic at no-space-before-quote positions. Byte-confirmed and read at 600 dpi; quote census 18 opening against 26 closing, an imbalance of exactly these four. Same class of fault as E21 on p.ix, and evidence it is a typesetting behaviour rather than a one-off slip. |
| E24 | 7 | 19 | 02 ability scores and races | HALFLINGS, `Languages:` — *"a halfling may learn an additional language, but **may not more** than two additional languages regardless of intelligence."* A verb is omitted after "may not". The parallel gnome entry on p.5 reads *"They may not **learn** more than two…"*, which is what makes the omission legible as an omission rather than an odd construction. Confirmed at 600 dpi; no clipped or overset glyph. |
| E25 | 10 | 22 | 03a character classes | Cleric introduction prints **`estab-lishes`** with the hyphen **mid-line** — `Whether the cleric estab-lishes a stronghold or a temple,` all on one printed line, the word box at x 263.9–298.2 with the line continuing to the column edge at x 371.7. This is a printed hyphen, **not** the line-break extraction artefact the leave-alone list describes; that ruling was made about a different instance and does not cover this one. The same word is set correctly as `establishes` 36 pt higher on the same page, at a line end, unhyphenated. Read at 600 dpi and confirmed from word-box geometry. See the narrowed `estab/lishes` note in the leave-alone list. |
| E26 | 18 | 30 | 03b character classes | Magic User introduction: `Nevertheless, those character who possess formidable intelligence…` — singular *character* where the plural belongs. |
| E27 | 18 | 30 | 03b character classes | Same page: `normally may only cast spell they have learned from these books` — singular *spell* where the plural belongs. Distinct from E26 and separately marked. |
| E28 | 19 | 31 | 03b character classes | Magic User To Hit table span label prints `Roll required to hit Armour Class` in mixed case. A census of every such label in book pp.8–27 returns eleven: ten set `ROLL REQUIRED TO HIT ARMOUR CLASS` in full caps (book pp.10, 12, 14, 15, 16, 17, 21, 22, 24, 27) and this one alone in mixed case. |
| E29 | 31 | 43 | 04 alignment money equipment | EQUIPMENT introduction prints `Players should check with their GM whether  the prices show below apply…` — **`show`** for *shown*, and a **double space** after `whether`. The space measures 2.72 pt against roughly 1.32 pt for every other word gap on the same line. 600 dpi and geometrically confirmed. |
| E30 | 28 | 40 | 04 alignment money equipment | ALIGNMENT introduction prints `If a barbarian comes from a  society that kills the weak` — a **double space** mid-line after `a`. The gap measures 3.05 pt against a uniform 1.49 pt for the eleven other word gaps on the same justified line. 600 dpi and geometrically confirmed. |
| E31 | 10 | 22 | 03a character classes | Cleric introduction, the same sentence that carries E25: `followers and  acolytes` — a **double space**, gap 2.71 pt against 1.32 pt for every other gap on the line. |
| E32 | 11 | 23 | 03a character classes | Turning Undead paragraph: `in the  descriptions` — a **double space**, gap 2.28 pt against a 1.10 pt line median. |
| E33 | 14 | 26 | 03a character classes | FIGHTER introduction: `whether  on offence` — a **double space**, gap 2.26 pt against a 1.09 pt line median. The same post-`whether` slip as E29. |
| E34 | 2 | 14 | 02 ability scores and races | Constitution section: `certain spells of the illusion type (whether  cast by` — a **double space**, gap 2.69 pt against a 1.31 pt line median. Found by the wide-gap back-fill scan; had been normalised in transcription and was restored. |
| E35 | 22 | 34 | 03b character classes | Ranger restrictions: `may travel or operate together  at any one time.` — a **double space**, gap 2.72 pt against 1.32 pt. Back-fill scan find; restored. |
| E36 | 22 | 34 | 03b character classes | Ranger combat: `one attack at 1st to 7th  level, 3/2 attacks` — a **double space**, gap 3.15 pt against 1.56 pt. The paladin's parallel sentence on p.20 prints the same phrase with a normal 0.96 pt gap. Back-fill scan find; restored. |
| E37 | 25 | 37 | 03b character classes | Thief introduction: `even found  working on the side of the law` — a **double space**, gap 2.15 pt against 1.01 pt. Back-fill scan find; restored. |
| E38 | 36 | 48 | 05 spells overview | Explanatory notes, half-damage example: `with fireball if the saving throw is halved, targets within the area of effect take half the damage` — **`halved`** where *passed* belongs. The sentence's own preceding definition reads "if the saving throw is passed, the spell takes half-effect". Verified at 600 dpi. |
| E39 | 42 | 54 | 06a spells cleric | Augury (entry opens on p.41; the flagged sentence is at the top of p.42 col 1): `whether  a` — a **double space**, gap 2.24 pt against a 1.08 pt line median. Page attribution corrected from 41/53 by the batch-3 audit. |
| E40 | 42 | 54 | 06a spells cleric | Bless: `enemies with—5% morale` — an **em dash (U+2014) closed up** against both words where a minus with space belongs; the same line prints `–1` with a proper en dash (U+2013). |
| E41 | 44 | 56 | 06a spells cleric | Detect Charm: `whether  a` — a **double space**, gap 3.11 pt against 1.52 pt. |
| E42 | 45 | 57 | 06a spells cleric | Detect Lie: `whether  the` — a **double space**, gap 3.04 pt against 1.48 pt. |
| E43 | 45 | 57 | 06a spells cleric | Divination: `if a  legendary` — a **double space**, gap 3.24 pt against 1.62 pt. |
| E44 | 47 | 59 | 06a spells cleric | Heal: `will negates the effects` — **`negates`** where *negate* belongs. |
| E45 | 48 | 60 | 06b spells cleric | Holy Word effect table, 12+ HD row: `(duration 1- 4 rounds)` — a **space inside the range** `1- 4`, where the parallel rows print `10-40`, `2-8` closed up. Separate word boxes with a normal word gap. |
| E46 | 48 | 60 | 06b spells cleric | Light: `a penalty of -4` — an **ASCII hyphen** where the range's six other penalty values print en-dashes (–4, –2, –1). |
| E47 | 51 | 63 | 06b spells cleric | Remove Curse curse table: `in the case of an non-tool-using creature` — **`an`** before a consonant. |
| E48 | 52 | 64 | 06b spells cleric | Restoration: `Level: 7` — a bare `7` where the other cleric entries print `Cleric N`. Logged as an inconsistency, E22-style; possibly deliberate. Reproduced as printed. |
| E49 | 52 | 64 | 06b spells cleric | Resurrection: `Level: 7` — same fault as E48 in the adjacent entry. Distinct and separately marked. |
| E50 | 53 | 65 | 06b spells cleric | Speak with Animals: `the  conversation` — a **double space**, 2.2× the line median, confirmed at 600 dpi. |
| E51 | 62 | 74 | 07 spells druid | Hallucinatory Forest: the school line `Druidic Illusion/ Phantasm` is set in the **regular body face** (MyriadPro-SemiCn 11 pt) where all 77 other school lines in the chapter are italic (MyriadPro-It 12 pt). Font-verified. Same census class as E28. |
| E52 | 63 | 75 | 07 spells druid | Heat Metal: `divesting him-  or herself` — a **double space**, gap 2.15 pt against a 1.02 pt line median. Control: p.57 prints `him- or herself` with a normal single space. |
| E53 | 63 | 75 | 07 spells druid | Hold Plant: `can move, whether  naturally` — a **double space**, gap 2.34 pt against 1.13 pt. The fourth post-`whether` instance (with E29, E33, E34). |
| E54 | 66 | 78 | 07 spells druid | Protection From Fire: `casts it upon him-  or herself` — a **double space**, gap 2.82 pt against 1.37 pt. |
| E55 | 66 | 78 | 07 spells druid | Protection From Fire: `Any damage incurred by fire attacks will also reduced by half.` — the verb **be is absent**. Read at 600 dpi; word gap normal, no clipped glyph. Same class as E24. |
| E56 | 66 | 78 | 07 spells druid | Reincarnate: `the new race. The  character will retain` — a **double space** between `The` and `character` (mid-sentence, not the sentence gap), 2.9 pt against 1.4 pt. |
| E57 | 69 | 81 | 07 spells druid | Wall of Fire: `taking twice the ordinary  damage` — a **double space**, gap 2.6 pt against 1.25 pt. |
| E58 | vii / 339 | 9 / 351 | 01 lists + 26 rods staves wands armour swords | **The book contradicts itself between its own index and its body.** The front-matter List of Magic Items (book p.vii) prints `L Shield +1, Missile Deflector`; the body entry (book p.339) prints `Large Shield +1, Missile Deflector (CDFPR):`. Both confirmed at 600 dpi and by word box on 2026-09-06 — on p.vii `L` is its own 2.408 pt box (x 216.108–218.516); on p.339 `Large` is a single 17.3 pt box (x 48.000–65.3025). **Neither file is wrong: file 01 and file 26 each reproduce their own page correctly.** Do not harmonise them. |
| E59 | 325 / 333 | 337 / 345 | 25 treasure coin gems potions scrolls | **A generation table that does not match its own entries.** Master Magic Item Table III (“Scrolls Table 3: Scrolls of Warding”, book p.325) lists nine roll results including `01-02 Acid` and `17-18 Polymorph`. The book's actual named Scrolls of Warding, described in full on book p.333, are eight: Demons, Devils, Elementals, Lycanthropes, Magic, Petrifaction, **Possession**, Undead. **No Acid scroll exists anywhere in the book, and Possession stands where Polymorph would be.** Both sides raster-verified independently by audit batch 8 and its verifier. Reproduce both exactly as printed; do not harmonise either side. |
| E60 | viii | 10 | 01 lists (the omission) / 28 miscellaneous magic gog-z (the entries) | **The book's own List of Magic Items omits two entries that are fully printed and described in the body.** *Headband of Intellect* (book p.353, between Hat of Disguise and Helm of Brilliance) and *Portable Hole* (book p.358, between Plentiful Vessel and Restorative Ointment) appear in Chapter VI but not in the front-matter list. Confirmed by raw extraction of PDF 10 and a 300 dpi raster of the same page. **File 01 is not at fault** — it transcribes the list exactly as printed, including the omission — and file 28 carries both entries, which is why its roster came to 95 against the list's 93. Do not add the missing entries to file 01. |
| E61 | 70 | 82 | 08 spells magic user aff-for | Affect Normal Fires: `a holy symbol  or mistletoe as material components.` — a printed mid-sentence double space. Gap 2.72 pt against a uniform 1.32 pt for every other word gap on the same justified line. |
| E62 | 72 | 84 | 08 spells magic user aff-for | Cacodemon: `creatures of the nether  planes is, of course,` — a printed mid-sentence double space, gap 2.27 pt against a 1.10 pt line median. |
| E63 | 75 | 87 | 08 spells magic user aff-for | Contact Other Plane: `the being contacted will have the  knowledge the magic user seeks` — a printed mid-sentence double space, gap 2.28 pt against a 1.10 pt line median. |
| E64 | 78 | 90 | 08 spells magic user aff-for | Dimension Door: `cannot act for a period of 6 segments  following the transition.` — a printed mid-sentence double space, gap 2.72 pt against a 1.32 pt line median. |
| E65 | 78 | 90 | 08 spells magic user aff-for | Distance Distortion closes with the sentence `Otherwise, the spell is utterly undetectable.` printed twice in immediate succession — the first instance broken across a line as `un-`/`detectable.`, the second set whole on the following line. |
| E66 | 80 | 92 | 08 spells magic user aff-for | False Trap: the school line `Arcane Illusion/Phantasm` is set in the regular body face (MyriadPro-SemiCn 7.5 pt) where every other school line on the same page is italic (MyriadPro-It 8 pt). Same census class as E51. |
| E67 | 82 | 94 | 08 spells magic user aff-for | Fire Shield: `depending upon whether  the magic user elects` — a printed mid-sentence double space, gap 3.02 pt against a 1.47 pt line median. The same post-`whether` slip as E29, E33, E34, E39, E41, E42 and E53. |
| E68 | 86 | 98 | 09 spells magic user fre-per | Guards and Wards, suggestion clause: `The caster selects an area of  up to 5 ft square` — a printed mid-sentence double space, gap 2.06 pt against a 0.96 pt line median. |
| E69 | 90 | 102 | 09 spells magic user fre-per | Legend Lore, first paragraph: `until he can finally piece them together  into meaningful information` — a printed mid-sentence double space, gap 2.21 pt against a 1.06 pt line median. |
| E70 | 90 | 102 | 09 spells magic user fre-per | Legend Lore, second paragraph: `gather the legendary lore together  into a piece of true information` — a printed mid-sentence double space, gap 2.93 pt against a 1.43 pt line median. A second, distinct instance of the same phrase sixteen printed lines below the first (y 332.6 → 479.6 at a 9.0 pt line pitch). **Corrected on verification, 2026-09-07 — the first count said eleven.** |
| E71 | 91 | 103 | 09 spells magic user fre-per | Limited Wish: `or whether  the results of the request will suffer from flaws` — a printed mid-sentence double space, gap 3.13 pt against a 1.55 pt line median. Another post-`whether` instance. |
| E72 | 92 | 104 | 09 spells magic user fre-per | Magic Jar: `He or she does not gain any knowledge from the  creature’s mind` — a printed mid-sentence double space, gap 3.04 pt against a 1.49 pt line median. |
| E73 | 94 | 106 | 09 spells magic user fre-per | Mending: `It can weld together  broken metallic objects` — a printed mid-sentence double space, gap 3.30 pt against a 1.66 pt line median. |
| E74 | 95 | 107 | 09 spells magic user fre-per | Mirror Image: `it is randomly determined whether  the to-hit roll is directed` — a printed mid-sentence double space, gap 3.17 pt against a 1.58 pt line median. Another post-`whether` instance. |
| E75 | 97 | 109 | 09 spells magic user fre-per | Move Earth: `although the spell cannot  move rock unless the rock is carried` — a printed mid-sentence double space, gap 3.44 pt against a 1.73 pt line median. |
| E76 | 99 | 111 | 10 spells magic user pha-wri | Polymorph Self: `Changing from one shape to  another requires only 30 seconds` — a printed mid-sentence double space, gap 2.40 pt against a 1.16 pt line median. |
| E77 | 99 | 111 | 10 spells magic user pha-wri | Polymorph Self: `he or she would be able to use whatever weapons he or she  could use` — a printed mid-sentence double space, gap 2.58 pt against a 1.25 pt line median. |
| E78 | 99 | 111 | 10 spells magic user pha-wri | Power Word Kill: `the magic user specifies whether  the spell is to kill one creature` — a printed mid-sentence double space, gap 3.07 pt against a 1.51 pt line median. Another post-`whether` instance. |
| E79 | 103 | 115 | 10 spells magic user pha-wri | Secret Chest: `have a craftsman or craftsmen build it, together  with a second, miniature copy` — a printed mid-sentence double space, gap 2.78 pt against a 1.34 pt line median. |
| E80 | 103 | 115 | 10 spells magic user pha-wri | Secret Chest: `the chest disappears into the æthereal plane, together  with its contents` — a printed mid-sentence double space, gap 3.02 pt against a 1.47 pt line median. A second, distinct instance three printed lines below the first. |
| E81 | 105 | 117 | 10 spells magic user pha-wri | Spider Climb: `The subject of this spell will  find it difficult to employ tools` — a printed mid-sentence double space, gap 2.84 pt against a 1.38 pt line median. |
| E82 | 106 | 118 | 10 spells magic user pha-wri | Stone Shape: `Whether  used to decorate the wizard’s tower with gargoyles` — a printed mid-sentence double space, gap 3.12 pt against a 1.55 pt line median. |
| E83 | 114 | 126 | 11 spells illusionist | Deafness: the stat-block label `Area of Effect:` is set in the regular body face (MyriadPro-SemiCn) where every other stat label on the page — including the `Level:` / `Range:` / `Duration:` immediately above it in the same block — is MyriadPro-SemiboldSemiCn. One exception in a census of 56 labels on the page (eight blocks of seven), and one of eight `Area of Effect:` labels. **Counts corrected on verification, 2026-09-07 — the first census said 32 and nine.** |
| E84 | 114 | 126 | 11 spells illusionist | Demi-Shadow Magic: the spell list reads `cloudkill, cone of cold, magic missile, fireball, lighting bolt, wall of fire, wall of ice` — `lighting` for *lightning*. The book sets *Lightning Bolt* correctly as a magic user spell heading on book p.90 and in the front-matter List of Spells. |
| E85 | 116 | 128 | 11 spells illusionist | Hypnotism: `The only indication about whether  a creature has been affected` — a printed mid-sentence double space, gap 3.18 pt against a 1.58 pt line median. Another post-`whether` instance. |
| E86 | 128 | 140 | 12 time movement combat | COMBAT MODIFIERS, Cover: the four-line cover-bonus list prints `25% cover: -2 AC`, `50% cover: -4 AC`, `75% cover: -7 AC` and then `90% cover -10 AC` — the fourth line alone lacks the colon its three siblings carry. |
| E87 | 130 | 142 | 12 time movement combat | TURNING THE UNDEAD notes: `It the table indicates “D”, the undead creature is automatically destroyed` — `It` for *If*. The immediately preceding sentence on the same page reads `If the table indicates “T”, the undead creature is automatically turned`, which is what makes the slip legible as an error. |
| E88 | 136 | 148 | 13 hirelings and henchmen | The descriptive heading prints `Engineer (Miner and Sapper):` where the wage table on book p.134 prints `Engineer (Miner or Sapper)` for the same hireling. The book contradicts itself between a table and its own description; both are reproduced as printed. |
| E89 | 144 | 156 | 13 hirelings and henchmen | Loyalty Test table, `> 100` row: `Fanatical: Will serve unquestioningly and fight to the death` closes with no full stop. The table's five other rows all end with one. |
| E90 | 146 | 158 | 14a exploration town planes | Wandering Monsters: `special provisions for wandering monsters affecting  the frequency of checks` — a printed mid-sentence double space, gap 3.17 pt against a 1.58 pt line median. |
| E91 | 146 | 158 | 14a exploration town planes | Wandering Monsters: `there is no incentive for the players to keep the game moving no reason why they shouldn’t hold long conversations` — no punctuation between the two clauses. The same paragraph's closing sentence sets the parallel construction with an em dash: `keep the game moving—otherwise the game will become mired`. |
| E92 | 150 | 162 | 14a exploration town planes | Ad-hoc rulings: the opening quotation mark before `you succeed` is set as a CLOSING mark (U+201D) where an opening mark belongs. Same fault class as E21 and E23, and at the same no-space-before-quote position E23 describes. |
| E93 | 153 | 165 | 14b example dungeon and sample play | Map Key room 5: `Goods Storage:  the orcs keep in this cave` — lower case after the colon where the four preceding rooms all capitalise (`1. Guard Cave:  The`, `2. Common Sleeping Area:  All`, `3. Arsenal:  Assorted`, `4. Dog Kennel:  The`). |
| E94 | 155 | 167 | 14b example dungeon and sample play | Sample Play Session, Bob's marching-order speech: `the clEric has his hammer and shield` — a mid-word capital E. The same speech sets `cleric` correctly two sentences earlier (`with the cleric bringing up the rear`). |
| E95 | 155 | 167 | 14b example dungeon and sample play | Sample Play Session: `The 2 orcs on Floppinjay follow him north and attack [roll] 1 miss, 1 hit.` — the stage direction is singular `[roll]` where every other die-rolling stage direction in the transcript is plural. A census of book pp.155–156 returns 26 `[rolls]` (12 on p.155, 14 on p.156) against this single `[roll]`, plus `[rolls reaction die]`. |
| E96 | 157 | 169 | 15 dungeons and generation | DUNGEONS, worked Example #1: the opening quotation mark is set as a CLOSING mark (U+201D) where an opening mark belongs. Same fault class as E21 and E23. |
| E97 | 157 | 169 | 15 dungeons and generation | DUNGEONS, worked Example #2: the opening quotation mark is set as a CLOSING mark (U+201D) where an opening mark belongs. Second of two on the page; distinct from seq 36 and separately marked. |
| E98 | 171 | 183 | 15 dungeons and generation | Monster Level Nine encounter table: `12-30 Otyugh, Greater` is followed by `26-40 NPC Party – see Sub-table` — the two ranges both cover 26–30. The parallel Monster Level Ten table on the same page prints the same two entries as a clean `12-15 Otyugh, Greater` / `16-20 NPC Party`, which is what makes the Level Nine pair legible as an error rather than a deliberate weighting. |
| E99 | 173 | 185 | 15 dungeons and generation | Party Magic Items Sub-Table 4, row 61-65: `Amulet of Natural Armour  +4 (any)` — a printed mid-cell double space, gap 2.18 pt against a 1.06 pt median for the row's other word gaps. |
| E100 | 174 | 186 | 16a urban and wilderness encounters | Nighttime Encounters table, row 26 keys its entry `Druid¹` with a superscript one, but no footnote keyed ¹ is printed anywhere on book pp.173–178; the two footnotes under both encounter tables are keyed `*` and `**`, and the parallel Daytime Encounters row 26 on p.175 keys the same entry `Druid*`. |
| E101 | 174 | 186 | 16a urban and wilderness encounters | The sub-table's own heading on p.174 is printed `Red-light Professions` (hyphenated, lower-case *light*) while both encounter tables cross-refer to it as `Red Light Professions` (two capitals, no hyphen) — p.174 row 44-50 and p.176 row 40-41. |
| E102 | 175 | 187 | 16a urban and wilderness encounters | Daytime Encounters table, row 19-21: a printed mid-sentence double space between `and` and `2d4`. |
| E103 | 176 | 188 | 16a urban and wilderness encounters | Daytime Encounters table, row 99 (Weretiger): a printed mid-sentence double space between `encountered` and `in`. |
| E104 | 178 | 190 | 16a urban and wilderness encounters | Wetlands Type-of-Encounter table: the NPC row is printed `58` and the Undead row immediately below it `58-60`, so a roll of 58 is assigned to two results. |
| E105 | 178 | 190 | 16a urban and wilderness encounters | Same Wetlands table, second overlap: the Water row is printed `81-95` and the Special row `95-00`, so a roll of 95 is assigned to two results. Distinct from the 58 overlap and separately marked. |
| E106 | 179 | 191 | 16b wilderness encounter tables | Aquatic terrain table, roll 20: `Rakshasha` with an intruded *h*, against `Rakshasa` set correctly at pp.184 and 187 in the same file and in the Chapter V monster entry. |
| E107 | 181 | 193 | 16b wilderness encounter tables | Desert terrain table, roll 18: the second instance of `Rakshasha`. Distinct from the p.179 instance and separately marked. |
| E108 | 186 | 198 | 16b wilderness encounter tables | Marine terrain table, roll 4: a printed double space inside the cell, between `Gnoll` and `(S5,`. |
| E109 | 189 | 201 | 16b wilderness encounter tables | Rural terrain table, roll 18: `Will o’the Wisp` — spaced and unhyphenated — against ten instances of `Will-o-the-Wisp` elsewhere in the same file. |
| E110 | 190 | 202 | 16b wilderness encounter tables | Tundra terrain table, roll 11: `Portuguese Man O’War` closed up, against `Portuguese Man O’ War` spaced at p.180. Two instances in the file, set two ways. |
| E111 | 191 | 203 | 16b wilderness encounter tables | Flying Dinosaurs sub-table: the 1d6 column is printed 1, 2, 4-5, 5, 6 — five rows for a nominal d6, with no row 3 and 5 assigned twice. |
| E112 | 193 | 205 | 17a monsters statistics men demi-humans | MEN introduction: a printed mid-sentence double space between `categories` and `below.` |
| E113 | 196 | 208 | 17a monsters statistics men demi-humans | Pilgrim entry, Thieves paragraph: `per every 10 pilgrim` — singular, against `per every 10 pilgrims` in the Fighters paragraph three lines above and in the Magic users paragraph three lines below. Class of E26/E27. |
| E114 | 196 | 208 | 17a monsters statistics men demi-humans | Pilgrim alignment d% table: the neutral row is printed `56—66` and the chaotic evil row `65—80`, so rolls of 65 and 66 are assigned to two alignments. |
| E115 | 196 | 208 | 17a monsters statistics men demi-humans | Pilgrim entry: `will be travel` — a participle is absent after `be` (or `be` is surplus). Class of E24/E55. |
| E116 | 196 | 208 | 17a monsters statistics men demi-humans | Pilgrim Treasure list: `Pilgrims (ea.)::` — a doubled colon. Four of the five labels in the list are set this way; `Magic users (ea.):` takes a single colon, which is the control that makes the doubling legible as an error. |
| E117 | 196 | 208 | 17a monsters statistics men demi-humans | Pilgrim Treasure list: `Fighters (ea.)::` — a doubled colon. Four of the five labels in the list are set this way; `Magic users (ea.):` takes a single colon, which is the control that makes the doubling legible as an error. |
| E118 | 196 | 208 | 17a monsters statistics men demi-humans | Pilgrim Treasure list: `Clerics (ea.)::` — a doubled colon. Four of the five labels in the list are set this way; `Magic users (ea.):` takes a single colon, which is the control that makes the doubling legible as an error. |
| E119 | 196 | 208 | 17a monsters statistics men demi-humans | Pilgrim Treasure list: `Thieves (ea.)::` — a doubled colon. Four of the five labels in the list are set this way; `Magic users (ea.):` takes a single colon, which is the control that makes the doubling legible as an error. |
| E120 | 196 | 208 | 17a monsters statistics men demi-humans | Merchant entry: `led by higher level fighter` — the article is absent before a singular noun. The same page's parallel constructions read `a magic user of 6th to 8th level`, `a cleric of 5th to 7th level`, `a thief of 8th to 10th level`; and the two other `led by higher level fighters` on p.195 are plural, where no article is needed. Class of E24/E55. |
| E121 | 196 | 208 | 17a monsters statistics men demi-humans | Merchant Treasure, Individual Merchants line: `1d6x10` set with an ordinary lower-case x where every other multiplier on the page uses `×` (e.g. `1d6×100 pp`, `1d6×10 gems` in the Bandit Treasure line at the head of the same page). |
| E122 | 196 | 208 | 17a monsters statistics men demi-humans | Merchant Treasure, Mercenary Pay Box line: an unmatched closing parenthesis after `4d4 gems`. The line opens three parentheses and closes four. |
| E123 | 198 | 210 | 17a monsters statistics men demi-humans | Elf entry: `and elf` where *an elf* belongs. The same entry prints `An elf’s appearance` and `the life span of an elf`. |
| E124 | 198 | 210 | 17a monsters statistics men demi-humans | Gnome entry: `higher then` for *higher than*. |
| E125 | 199 | 211 | 17a monsters statistics men demi-humans | Halfling entry, TWO distinct defects on one line: (1) `higher then` for *higher than*, the second instance of the p.198 fault; (2) `very adapt` for *very adept* — the control is two sentences later on the same page, `Halflings are so adept at using the natural camouflage`. |
| E126 | 199 | 211 | 17a monsters statistics men demi-humans | Halfling entry, TWO distinct defects on one line: (1) `higher then` for *higher than*, the second instance of the p.198 fault; (2) `very adapt` for *very adept* — the control is two sentences later on the same page, `Halflings are so adept at using the natural camouflage`. |
| E127 | 202 | 214 | 17b monsters humanoids giants | Goblin Treasure line: a printed space before the semicolon. Class of E18. |
| E128 | 204 | 216 | 17b monsters humanoids giants | Orc Treasure line: the same printed space before the semicolon. |
| E129 | 205 | 217 | 17b monsters humanoids giants | GIANT introduction: `so long it is within their interests` — *as* is absent before `long`. Class of E24/E55. |
| E130 | 206 | 218 | 17b monsters humanoids giants | Giant, Fire description: `The` where *They* belongs — the sentences either side of it use `their`/`Their`. |
| E131 | 208 | 220 | 17b monsters humanoids giants | Ettin Treasure line: no comma or conjunction between `1d4 jewellery (20%)` and `2 magic items`, against every parallel Treasure line in the file, which comma-separate every element. |
| E132 | 210 | 222 | 17b monsters humanoids giants | Troll, Giant: a singular verb on a plural subject — `giant trolls attack twice per round … and is easily capable`. Class of E26/E27. |
| E133 | 210 | 222 | 17b monsters humanoids giants | Troll, Giant Two-Headed: `the others stays alert` — singular verb on a plural subject. Distinct from the Troll, Giant fault and separately marked. |
| E134 | 211 | 223 | 18 monsters dragons and demons | Troll, Spectral: the verb *be* is absent after `would`. Class of E24/E55. |
| E135 | 212 | 224 | 18 monsters dragons and demons | Dragon, Blue: `lighting` for *lightning*. The Bronze dragon's parallel sentence on p.213 prints `a bolt of lightning`, which is what makes it legible as a slip. |
| E136 | 217 | 229 | 18 monsters dragons and demons | Demons introduction: `a` before a vowel. Class of E47. |
| E137 | 217 | 229 | 18 monsters dragons and demons | Attack Form table, Silver row: no space before the opening parenthesis. |
| E138 | 218 | 230 | 18 monsters dragons and demons | Babau: the paragraph ends with no terminal full stop. |
| E139 | 218 | 230 | 18 monsters dragons and demons | Babau: a sentence opening with a lower-case `class`, immediately after `…despised by class A, B and C demons.` |
| E140 | 219 | 231 | 18 monsters dragons and demons | Glabrezu: a full word space before the closing parenthesis. Class of E18. |
| E141 | 220 | 232 | 18 monsters dragons and demons | Demon, Class E: two faults in one paragraph — a full word space before the closing parenthesis at `magic user spell )` (class of E18), and a full stop printed inside the closing parenthesis at `(50% chance of success.)`. |
| E142 | 221 | 233 | 18 monsters dragons and demons | Demon, Class F: two faults in one paragraph — a full word space before the closing parenthesis at `magic user spell )` (class of E18), and a printed mid-sentence double space at `gate  (as`. |
| E143 | 222 | 234 | 18 monsters dragons and demons | Demonette: `a victims life` — the possessive apostrophe is absent. The book sets `victim’s` on pp.211 and 223. |
| E144 | 222 | 234 | 18 monsters dragons and demons | Dretch: a printed mid-sentence double space at `gate  (as`. |
| E145 | 223 | 235 | 18 monsters dragons and demons | Ekivu: a printed mid-sentence double space at `gate  (as`. The third and last member of the p.221/222/223 set. |
| E146 | 223 | 235 | 18 monsters dragons and demons | Quasit: `a … monsters` — singular article against a plural noun. Class of E26/E27. |
| E147 | 224 | 236 | 18 monsters dragons and demons | Shub Treasure paragraph: the creature name is capitalised mid-sentence, against the lower-case `shub` used mid-sentence in the rest of the entry. |
| E148 | 225 | 237 | 18 monsters dragons and demons | Succubus: no space between the closing parenthesis and `or`. |
| E149 | 226 | 238 | 19 monsters devils dinosaurs golems | DEVILS introduction, abilities list: the parenthesis opened at `(varies,` is never closed — the sentence ends at `monster summoning I.` with the bracket still open. |
| E150 | 226 | 238 | 19 monsters devils dinosaurs golems | DEVILS introduction: fourteen words repeated verbatim — `its home plane in Hell for 9 decades of servitude as a lemure before` — with the pronoun switching from singular to plural across the seam. |
| E151 | 229 | 241 | 19 monsters devils dinosaurs golems | Ice Devil Treasure line: a printed space before the comma. Class of E18. |
| E152 | 231 | 243 | 19 monsters devils dinosaurs golems | Scaly Devil: the sentence names the creature twice over — `The scaly devils known as the scaly devil are quite common…`, plural subject and singular apposition. |
| E153 | 233 | 245 | 19 monsters devils dinosaurs golems | Tyrannosaurids and Allosaurids table: the Tyrannosaurus column's Special Defences cell is genuinely blank, where the other five columns and the Special Attacks row above all print `None`. |
| E154 | 235 | 247 | 19 monsters devils dinosaurs golems | Sauropods identification paragraph ends with no terminal full stop; the `Treasure:` line follows directly. |
| E155 | 235 | 247 | 19 monsters devils dinosaurs golems | Ceratopsians: the table's column header prints `Diceratus` and the identification paragraph on the same page prints `Diceratops:` — the same animal spelled two ways on one page. (The name is also set `Diceratops` in the p.191 Ceratopsians sub-table in file 16b.) The marker sits on the entry's prose line rather than in the table row, because an HTML comment on its own line inside a GFM table body terminates the table. |
| E156 | 236 | 248 | 19 monsters devils dinosaurs golems | Other Dinosaurs I introduction: a doubled full stop. |
| E157 | 237 | 249 | 19 monsters devils dinosaurs golems | Flying Dinosaurs table: eleven consecutive rows — Armour Class through Level/XP — are printed identical, column for column, to the first five columns of the Marine Dinosaurs table directly above, including `Swallow whole` as a Special Attack for two small flying reptiles. Only the four top rows (Frequency, No. Encountered, Size, Move) were rewritten for the flying species. |
| E158 | 237 | 249 | 19 monsters devils dinosaurs golems | Flying Dinosaurs: TWO same-page double spellings. The table's column headers print `Pteradon` and `Rhamphorynchus`; the identification paragraph six lines below prints `Pteranodon:` and `Rhamphorhynchus:`. The marker sits on the entry's prose line rather than in the table header row, because an HTML comment on its own line inside a GFM table body terminates the table. |
| E159 | 238 | 250 | 19 monsters devils dinosaurs golems | Iron Golem: `(i.e.: ` — a colon after *i.e.* The book uses `i.e.` twenty-seven times and this is the only one followed by a colon. |
| E160 | 239 | 251 | 20 monsters sylvan and undead | `sparking waterfalls` — `sparking` where *sparkling* belongs. Printed with a soft line break as `sparking wa-terfalls`; the hyphen is an extraction artefact, the missing `l` is on the page. |
| E161 | 240 | 252 | 20 monsters sylvan and undead | `spites` for *sprites*. The book sets the creature name `sprites`/`sprite` five times (book pp.203, 240, 241, 241, 243), four of them inside this file's own range; this is the only `spites`. The four other `spite` in the book are the noun in *in spite of*. |
| E162 | 241 | 253 | 20 monsters sylvan and undead | `he will never been again` — a past participle standing where a verb phrase belongs. Read at 600 dpi: no clipped or overset glyph, normal word gaps. |
| E163 | 241 | 253 | 20 monsters sylvan and undead | `rather then` for *rather than*. Member of the book-wide `then`-for-*than* class: nine instances across book pp.198, 199, 241, 246, 260, 265, 286, 287, 290, against 465 correct `than`. |
| E164 | 242 | 254 | 20 monsters sylvan and undead | The noun *chance* is absent after `75%`. The file's only two `% chance` constructions are the two defective ones (`a 75% the`, p.242, and `a 50% for`, p.249); every other percentage in the range is a bare stat value, so the control is the construction itself, not a count. |
| E165 | 242 | 254 | 20 monsters sylvan and undead | Possessive apostrophe absent in `the nixies short stature` (*nixies'*). The only construction of this shape in either file — a scan for `the <plural> <adjective>` across both returns this and nothing else. The book sets possessive apostrophes correctly throughout the range (`the frog's weight`, `the poltergeist's bond`, `the shadows' horrid ties`, 22 curly apostrophes in this file alone, all position-verified by the batch-6 audit). |
| E166 | 242 | 254 | 20 monsters sylvan and undead | Mid-sentence capital `Nymph`. The control is on the same page two lines above, in the immediately preceding sentence: `should a nymph be seen unclothed`. Census over the file: five lowercase mid-sentence `nymph` and three `nymphs`; every other capitalised `Nymph`/`Nymphs` is at a sentence start, in a heading, or in the roster line. One mid-sentence capital against eight lowercase. |
| E167 | 243 | 255 | 20 monsters sylvan and undead | A hyphen printed **mid-line**, with a space after it and the line continuing — E25 class, not the line-break extraction artefact the leave-alone list covers. Two lines above, the same page sets `a good aligned character` with no hyphen at all (its `char-acter` break is a soft hyphen in the extraction, not on the page). |
| E168 | 246 | 258 | 20 monsters sylvan and undead | `more then` for *more than*. Second instance in this file; member of the nine-strong book-wide class. |
| E169 | 246 | 258 | 20 monsters sylvan and undead | `addition` where *additional* belongs. The same paragraph two lines above prints `they cause an additional 1d6 damage`. |
| E170 | 246 | 258 | 20 monsters sylvan and undead | Ghast Treasure line: `d12×1,000` with no leading `1`. Four correctly-formed neighbours in the same two lines — `1d8×1,000 cp`, `1d6×1,000 sp`, `1d4×1,000 ep` before it and `1d6×1,000 pp` after. |
| E171 | 246 | 258 | 20 monsters sylvan and undead | Ghost Frequency set in title case. Re-derived census over the file's owned range: **eight `Very rare` against two `Very Rare`** (Ghost p.246, Lich p.247), identical position for position in the file and the PDF text layer. |
| E172 | 246 | 258 | 20 monsters sylvan and undead | Ghost XP printed without a thousands comma. The file's other six four-digit-and-up XP values all carry one — 1,295 and 3,600 (Treant sub-list), 1,300, 10,000, 1,815, 3,810. Six against this one. |
| E173 | 247 | 259 | 20 monsters sylvan and undead | `able travel` — the infinitive marker *to* is absent. Read at 600 dpi; word gaps normal, no clipped glyph. |
| E174 | 247 | 259 | 20 monsters sylvan and undead | Lich Frequency in title case — the second of the two capitalised instances against eight `Very rare` in range. Distinct from the Ghost instance and separately marked. |
| E175 | 247 | 259 | 20 monsters sylvan and undead | `at at` — the preposition doubled. The only doubled word in either file's range that is not a stat-block column value repeated across variants. |
| E176 | 248 | 260 | 20 monsters sylvan and undead | The relative pronoun is absent after `those mortals`, leaving two finite verbs with one subject. E24/E55 class — a dropped word, not an odd construction. Read at 600 dpi; word gaps normal, no clipped glyph. |
| E177 | 248 | 260 | 20 monsters sylvan and undead | Lich Treasure line: `(d4+1)` with no leading `1`. Two correctly-formed parenthesised parallels bracket it — `(1d4+1)×1,000 cp (30%)` on the same line and `(1d8+1)×1,000 gp (45%)` next. Same class as the Ghast line on p.246. |
| E178 | 248 | 260 | 20 monsters sylvan and undead | Mummy turning note with a capital `T`. **Re-derived census: fifteen lowercase `(turned as type N)` against two capitalised**, counted independently in the file and in the PDF text layer and identical case position for position; both capitals are on book p.248 (Mummy and Poltergeist). The register's earlier supporting figure of nine lowercase was wrong. |
| E179 | 248 | 260 | 20 monsters sylvan and undead | Poltergeist turning note with a capital `T` — the second of the two capitals against fifteen lowercase. Distinct from the Mummy instance and separately marked. |
| E180 | 248 | 260 | 20 monsters sylvan and undead | A stray article: `as a turning a type 3 undead`, where the sense requires `as turning as a type 3 undead` or similar. Reproduced as printed; the intended wording is not recoverable from the page. |
| E181 | 249 | 261 | 20 monsters sylvan and undead | The noun *chance* is absent after `50%`. Same fault as the Nixie line on p.242, in the same file. |
| E182 | 249 | 261 | 20 monsters sylvan and undead | Mid-sentence capital `Shadow`. Controls in the same paragraph: `shadows` lowercase three times and `shadow` once, all mid-sentence; the only other capitalised forms are the heading, the roster line and a sentence-initial `Shadows`. One mid-sentence capital against four lowercase in the same entry. |
| E183 | 249 | 261 | 20 monsters sylvan and undead | A hyphen printed **mid-line** inside `night-mares`, with the line continuing past it — E25 class. The control sits on the same printed line, which ends `physi-` at a genuine line break: the extraction carries a soft hyphen there and a hard one here. |
| E184 | 249 | 261 | 20 monsters sylvan and undead | Shadow's Treasure label printed without its colon. Census over this file: **twenty-nine `Treasure:` against this one bare `Treasure`**; file 21 has forty-nine, all with the colon. The label is set in the same italic semibold form as the rest. |
| E185 | 249 | 261 | 20 monsters sylvan and undead | `speak … of … can animate` — a subordinate clause with no complementiser, leaving the sentence without a working structure. Reproduced as printed; no repair is recoverable from the page. |
| E186 | 250 | 262 | 20 monsters sylvan and undead | `no affect` where the noun *effect* belongs. The same page uses `affect` correctly as a verb three times, including `enchantments that affect the mind have no power over spectres` in the adjacent entry. |
| E187 | 250 | 262 | 20 monsters sylvan and undead | Printed `(18.76)` with a baseline full stop, confirmed at 1500 dpi — not a solidus and not a clipped glyph. **But the book is self-consistent here:** a book-wide census returns four exceptional-strength values, all with a full stop (`18.76` book pp.229 and 250, `18.99` book pp.343 and 367), and **zero** instances of the `18/76` form anywhere. There is no in-book control that makes this legible as an error. |
| E188 | 252 | 264 | 20 monsters sylvan and undead | Verb agreement breaks part-way through a list. The subject is singular (`This type of zombie`) and takes three singular verbs — `moves`, `has`, `climbs` — before switching to plural `attack`, `use`, `can … use` for the rest of the sentence. Three agreeing verbs in the same sentence are the control. The marker is placed at the end of the sentence because the defect is the whole run from `attack` onward, not one word. |
| E189 | 253 | 265 | 21 monsters animals | Defect is on **line 92**, the Badger stat table's Frequency row, Giant column: `Very Rare` in title case. Census over this file: **eight `Very rare` against two `Very Rare`**, both capitals on book p.253 (this row and the prose sentence below). MARKER DISPLACED: the defect is inside a markdown table body, so per the placement rule the marker goes on the table's intro line — the `### Badger` heading — rather than in the row, which would terminate the table in GFM. |
| E190 | 253 | 265 | 21 monsters animals | A **second** title-case `Very Rare`, in the Giant Badger prose paragraph, mid-sentence. NEW FIND — the recorded list names only the table row. Both sit on book p.253; the file's other eight instances are all `Very rare`. |
| E191 | 254 | 266 | 21 monsters animals | Barracuda Size range with a capitalised second element. Census of every `X to Y` Size value in the monster chapter: `Small to medium` ×3 (book pp.260, 285, 303), `Small to large` ×2 (pp.297, 310), `Medium to large` ×2 (pp.264, 287) — **seven lowercase** — against `Small to Large` here and `Man-sized to Large` on book p.222 (a different file). Two of the seven controls are the same phrase in lowercase. NEW FIND; on neither recorded list. |
| E192 | 255 | 267 | 21 monsters animals | Two faults on one printed line: `2-6HD` closed up, and no terminal full stop. The parallel line in the very next entry (Boar, Warthog, book p.256) prints both correctly: `Young have the following stats: 1-2 HD, 1d4-1 or 1d4+1 damage.` HD-spacing census over this file: **twelve spaced `N HD` against this one closed-up `2-6HD`** (corrected on verification, 2026-09-07, from thirteen). Terminal-stop control: this is the only prose paragraph in either file that ends without terminal punctuation and is not a page-split continuation. Marker placed at line end because the missing stop is there; the `2-6HD` fault is on the same line and is covered by the same entry. |
| E193 | 260 | 272 | 21 monsters animals | `more then` for *more than*. The same paragraph prints `weighs less than the frog` and `weighs more than the giant frog` correctly two sentences earlier — two correct comparatives against this one, in the same paragraph. Member of the book-wide `then`-for-*than* class, **ten strong on a re-derived census** (book pp.197, 198, 199, 241, 246, 260, 265, 286, 287, 290) — corrected on verification, 2026-09-07, from nine. |
| E194 | 263 | 275 | 21 monsters animals | The entry heading prints `Man O’ War` with a space after the apostrophe; the body sets the name closed up **thirteen** times — twelve `man o’war` and one `men o’war`, all on the same page. **The recorded list says sixteen; the true count is thirteen.** Marker appended to the heading line (precedent: `30 compiled tables.md` carries two heading-line markers). |
| E195 | 265 | 277 | 21 monsters animals | Singular verb with a compound subject: `its tentacles and head is more vulnerable`. Reproduced as printed. NOTE: line 942 carries **two** candidates (this and `They only way`); the two insertions must be merged into one replacement of this line — applying either alone will make the other's `old_line` fail to match. |
| E196 | 265 | 277 | 21 monsters animals | `They` for *The*. Same line as the agreement fault above — see the merge note there. |
| E197 | 265 | 277 | 21 monsters animals | A verb is absent after `will` — E24/E55 class. The two parallel clauses in the same sentence are complete: `are 25% likely to have both arms held` and `will have one limb held`. The same defective sentence is reprinted verbatim in the Kraken entry on book p.290 (file 23a), so the fault is duplicated boilerplate, not a local slip. |
| E198 | 265 | 277 | 21 monsters animals | Two faults in four words: `looses` for *loses* and `more then` for *more than*. Book-wide census: **`looses` 2 against `loses` 23** — the other `looses` is the Kraken reprint of this same sentence on book p.290 (file 23a). `more then` is a member of the book-wide `then`-for-*than* class, **ten strong on a re-derived census** — corrected on verification, 2026-09-07, from nine. |
| E199 | 266 | 278 | 21 monsters animals | `every` for *ever*. NOTE: line 1050 carries **two** candidates (this and `can weight as much`); the two insertions must be merged into one replacement of this line. |
| E200 | 266 | 278 | 21 monsters animals | `weight` for *weigh*. Book-wide census: this is the **only** `weight` in the book used as a verb — the other 55 are the noun — against `weigh` **9** and `weighs` 9 (corrected on verification, 2026-09-07 — the first census said 10), one of which (`males weigh 80 to 100 lbs`, book p.267) is two entries later in this same file. Same line as `every more dangerous` — see the merge note there. |
| E201 | 267 | 279 | 21 monsters animals | Defect is on **line 1149**, the Wolverine stat table's Alignment row, both columns: `Neutral Evil` with a capital E. Census over the monster chapter: **`Neutral evil` 12 against `Neutral Evil` 4**, and all four capitals sit on just two pages — book p.192 (×2) and this row (×2). The nearest control is the very next entry, Worg on book p.268, which prints `Neutral evil`. NEW FIND; on neither recorded list. MARKER DISPLACED to the `### Wolverine` heading — the table's intro line — because the defect is inside a table body. |
| E202 | 273 | 285 | 22a monsters other a-cat | Bee, Giant royal-jelly paragraph prints “3d6x1,000 gp” with an ASCII lowercase x where every other dice multiplier in the range prints a multiplication sign; the same page sets “1d12×1,000” with a genuine ×, and at 1200 dpi the disputed glyph measures 49 px ink width / 60 px ink height against 64 / 65 for the real × and 49 / 60 for known lowercase x in “noxious” and “complexes” on the same page. |
| E203 | 274 | 286 | 22a monsters other a-cat | Beetle, Giant → Giant Water bold run-in prints “Hunting by scent an vibration” — “an” where “and” belongs. Same class as errata E24/E55. |
| E204 | 275 | 287 | 22a monsters other a-cat | Bulette description prints “have been know to dig” — the participle ending is absent; the very next paragraph prints the correct form, “They have been known to attack a well-armed party”, which is what makes it legible as an omission. |
| E205 | 276 | 288 | 22a monsters other a-cat | Caryatid Column prose omits the article before “sword”: “The only indication of their true nature is a faint outline of sword held in one hand.” Same class as errata E24. |
| E206 | 276 | 288 | 22a monsters other a-cat | Caryatid Column prose prints a clause with no subject for “reduces”: “For each plus that the weapon has reduces the chance of breaking by 5%;”. The preceding sentence supplies the base rate (“a 25% chance of breaking”), which is what makes the construction legible as broken rather than merely compressed. |
| E207 | 277 | 289 | 22b monsters other cen-gar | Centipede stat block, Special Defences row: all three variant columns print “None-” with a trailing hyphen and no continuation, where the same field prints a bare “None” in the Chimæra table on the same page and throughout the chapter. |
| E208 | 277 | 289 | 22b monsters other cen-gar | Chimæra Treasure line prints a double space between “jewellery” and “(10%)” — a mid-sentence gap between plain tokens, not a sentence-boundary or post-label gap. Gap 2.80 pt against a 1.36 pt line median (2.06×). |
| E209 | 277 | 289 | 22b monsters other cen-gar | Gorgimæra Treasure line prints the same double space between “jewellery” and “(15%)”. Gap 3.82 pt against a 1.95 pt line median (1.96×). |
| E210 | 278 | 290 | 22b monsters other cen-gar | Couatl stat block prints “Vary rare” for “Very rare”. A book-wide census finds “Vary rare” exactly twice — here and at the Crypt Thing on book p.279 — against 65 correctly-set “Frequency: Very rare” rows. |
| E211 | 278 | 290 | 22b monsters other cen-gar | Couatl Treasure line prints “2d19 gems (55%)”. A d19 is not part of the game's dice set and a book-wide search finds the string exactly once — here. The strongest of this file's unmarked candidates. |
| E212 | 279 | 291 | 22b monsters other cen-gar | Crypt Thing stat block prints “Vary rare” for “Very rare” — the second and last instance in the book. |
| E213 | 279 | 291 | 22b monsters other cen-gar | Crypt Thing prose prints “disappear-ance” with a printed mid-line hyphen. The word box runs x 221.88–266.17 at the START of its line and the line continues to x 383, so this is not a line-break extraction artefact. Same class as errata E25. |
| E214 | 279 | 291 | 22b monsters other cen-gar | Crypt Thing Treasure line prints “1d6×100pp” closed up, where the same field is set “…×100 pp” with a space at five other sites in this file's range — book p.277 Chimæra (1d8×100 pp) and Gorgimæra (1d10×100 pp), book p.278 Couatl (3d4×100 pp), and book p.282 twice (1d6×100 pp, 5d10×100 pp). |
| E215 | 279 | 291 | 22b monsters other cen-gar | Dakon prose prints “likely to be settle anywhere” — a broken verb phrase. Same class as errata E24/E55. |
| E216 | 279 | 291 | 22b monsters other cen-gar | Dakon Treasure line prints “1d10×100pp” closed up — the second instance of the Crypt Thing fault, on the same page, against five spaced siblings in the range. |
| E217 | 279 | 291 | 22b monsters other cen-gar | Dark Creeper / Dark Stalker stat table, No. Encountered row: the parenthetical is split across the two printed columns with mismatched delimiters — the Dark Creeper cell reads “1 (or 20d4,” with no closing parenthesis and the Dark Stalker cell reads “1 see below)” with no opening parenthesis and no comma. |
| E218 | 280 | 292 | 22b monsters other cen-gar | Dark creeper prose prints “the affects of darkness” — the noun form where “effects” belongs. Book-wide, “affects” appears **33** times, and **two** are nominal: this one and book p.332 (*Potion of Undead Control*, file 25), which prints “**The affects of** this potion last 5d4 rounds.” **Census corrected on verification, 2026-09-07 — the first census said 31 occurrences and one nominal use. Corrected again on 2026-09-07: the book p.332 instance is NOT unmarked — it carries a marker and is logged as E302.** |
| E219 | 280 | 292 | 22b monsters other cen-gar | Dark creeper prose prints “it body” for “its body”. Same class as errata E26/E27. |
| E220 | 280 | 292 | 22b monsters other cen-gar | Dark creeper prose omits “chance”: “…have an 80% of surviving this magical fire undamaged.” Same class as errata E24/E55. |
| E221 | 280 | 292 | 22b monsters other cen-gar | Dark stalker prose sets the spell name “wall of fog” in the regular body face (MyriadPro-SemiCn) where the same page sets its other spell references — “darkness”, and the creeper's “detect magic” — in italic (MyriadPro-SemiCnIt). Exactly the errata E51 class. |
| E222 | 281 | 293 | 22b monsters other cen-gar | Disenchanter stat block, Special Defences row: the preposition “by” is absent. The entry's own prose two paragraphs below reads “can only be hit by magic weapons”, which is what makes it legible as an omission. |
| E223 | 281 | 293 | 22b monsters other cen-gar | Doppelgänger Level/XP row spells the per-hit-point bonus out as “+ 3 per hp” where all twenty other Level/XP values in book pp.277–285 use the “+N/hp” form. |
| E224 | 282 | 294 | 22b monsters other cen-gar | The Elemental entry contradicts itself about the Air Elemental's damage: the stat table's Damage row prints 2d10 and the Air Elemental prose prints “a stream of air that they use like an invisible limb to strike for 2d20 damage”. Which side is wrong is not determinable from the page — reproduce both, as with errata E58/E59. The marker sits on the Air Elemental prose line rather than in the stat table's Damage row, because an HTML comment on its own line inside a GFM table body terminates the table. |
| E225 | 283 | 295 | 22b monsters other cen-gar | Earth Elemental prose omits the article: “against foes who are not in contact with ground”. The same sentence's earlier clause prints “in contact with the earth”, and the paragraph above prints “they remain in contact with the earth” — two controls on the page. |
| E226 | 284 | 296 | 22b monsters other cen-gar | Executioner's Hood stat block repeats the field's own unit inside its value: “Hit Dice: 3 to 6 hit dice”. Of 284 Hit Dice rows in the book only two do this, and **23** other rows print a bare “N to N” range (corrected on verification, 2026-09-07, from 25). |
| E227 | 285 | 297 | 22b monsters other cen-gar | Horsefly, Giant prose prints “is” for “it”: “it will land on any warm-blooded creature is encounters”. |
| E228 | 285 | 297 | 22b monsters other cen-gar | Fungi, Violet prose prints “if” for “of”: “each plant has 1d4 branches growing out if it.” |
| E229 | 286 | 298 | 23a monsters other gel-mer | Genie prose prints a double space between “noble” and “genie” — mid-sentence, between plain words. Gap 3.11 pt against a 1.54 pt line median (2.02×). |
| E230 | 286 | 298 | 23a monsters other gel-mer | Genie prose prints a double space between “any” and “intelligent”. Gap 2.71 pt against a 1.32 pt line median (2.05×). |
| E231 | 288 | 300 | 23a monsters other gel-mer | Hell Hound Level/XP block prints four rows labelled (4 HD), (5 HD), (5 HD), (7 HD) — the third duplicates the second where (6 HD) belongs. The stat block's own Hit Dice row reads “4 to 7”, and the XP progression 4/75, 5/110, 6/160, 7/225 runs one row per hit die. |
| E232 | 288 | 300 | 23a monsters other gel-mer | Hippogriff prose omits “with”: “Even though hippogriffs are omnivorous they do not mix well other winged beasts.” Same class as errata E24/E55. |
| E233 | 289 | 301 | 23a monsters other gel-mer | Hydra Damage row prints no space after the first comma and a space after the second: “1d6,1d8, 1d10 or 1d12”. “1d6,1d8,” is a single word box and “1d10” follows at a 1.32 pt word gap. Same class as errata E45. |
| E234 | 289 | 301 | 23a monsters other gel-mer | Hydra Treasure line prints a bare “p” where a coin abbreviation belongs; the same line prints “cp”, “ep” and “gp” correctly in the adjacent values. |
| E235 | 290 | 302 | 23a monsters other gel-mer | Invisible Stalker prose omits “of”: “attempting to twist the meaning its orders”. The next sentence prints “make its meaning airtight”, so the noun is right and the preposition is missing. |
| E236 | 290 | 302 | 23a monsters other gel-mer | Kraken prose omits “have”: “The other 25% of the time the victim will both arms free and can attack…”. The same paragraph's parallel clause prints “they will have one limb held”. |
| E237 | 290 | 302 | 23a monsters other gel-mer | Kraken prose names the wrong creature: “…and can attack the squid with only a -1 penalty”, inside the Kraken entry. |
| E238 | 291 | 303 | 23a monsters other gel-mer | Lammasu prose sets the spell name “dimension door” in the regular body face (MyriadPro-SemiCn) at its first occurrence, where the second occurrence four lines below is italic (MyriadPro-SemiCnIt). Same census class as errata E51. |
| E239 | 291 | 303 | 23a monsters other gel-mer | Lammasu spell list prints a double space inside “4—1st level, 3—2nd  level, 2—3rd level, 1—4th level.” — the only non-uniform gap on an otherwise perfectly even line. Gap 2.59 pt against a 1.24 pt line median (2.09×). |
| E240 | 291 | 303 | 23a monsters other gel-mer | Lammasu prose prints “an” before a consonant: “away from an flying opponent's path of attack”. Exactly the errata E47 class. |
| E241 | 291 | 303 | 23a monsters other gel-mer | Lamia Treasure line prints “1d8×100pp” closed up, the same fault as the two already-marked instances at book p.279 (Crypt Thing and Dakon, file 22b). Book-wide the closed-up form occurs exactly three times; the spaced form “×100 pp” is used everywhere else, including twice in this file's own range (book p.292 “1d4×100 pp”, book p.293 “1d6×100 pp”). |
| E242 | 292 | 304 | 23a monsters other gel-mer | Fire Lizard prose omits “of”: “False dragons are normally slow-moving creatures and spend 50% their time sleeping in their subterranean lairs.” |
| E243 | 292 | 304 | 23a monsters other gel-mer | Fire Lizard prose omits “to”: “their lairs tend be littered with coins and gems.” |
| E244 | 293 | 305 | 23a monsters other gel-mer | Locathah prose omits “chance”: “There is a 5% chance a sub-chief or war-chief will be carrying a magic weapon of the appropriate type and a 10% a full chief will have one.” The same sentence's first clause prints “a 5% chance”, which is the control. |
| E245 | 294 | 306 | 23a monsters other gel-mer | Mephit table, Move row, Lava column prints “(AA level IV)” where the Fire, Smoke and Steam columns in the same row print “(AA: IV)”. The long form occurs exactly once in the book against 86 instances of the “(AA:N)” form. The marker sits on the `Mephit` entry heading rather than in the Move row, for the same reason. |
| E246 | 295 | 307 | 23a monsters other gel-mer | Lava Mephit prose carries a stray verb: “Wood is dissolves a little more slowly, about an inch per hour of contact.” |
| E247 | 295 | 307 | 23a monsters other gel-mer | Mephit entry sets the Lava Mephit's “gate” in the regular body face where the same page sets the Fire, Smoke and Steam mephits' “gate” in italic. Same class as errata E51. |
| E248 | 295 | 307 | 23a monsters other gel-mer | Smoke Mephit prose prints “with” for “within”: “inflicts 1 point of damage to everyone with 10 ft, no saving throw allowed.” |
| E249 | 296 | 308 | 23b monsters other min-rem | Mongrelman stat block repeats the field's own unit inside its value: “Hit Dice: 1 to 4 hit dice”. Of 284 Hit Dice rows in the book only two do this — this one and Executioner's Hood at book p.284 (file 22b) — and **23** other rows print a bare “N to N” range (corrected on verification, 2026-09-07, from 25). |
| E250 | 297 | 309 | 23b monsters other min-rem | Naga table, Size row, Water column prints “Medium(10 ft long)” with no space before the parenthesis, where the Guardian and Spirit columns in the same row print “Large (20 ft long)” and “Large (15 ft long)” with a space. “Medium(10” is a single word box. The marker sits on the naga entry's intro line rather than in the Size row, because an HTML comment on its own line inside a GFM table body terminates the table. |
| E251 | 298 | 310 | 23b monsters other min-rem | Guardian naga description ends its paragraph with no terminal full stop: “…and the target must save vs poison or die”. Every other paragraph in the entry is stopped. |
| E252 | 298 | 310 | 23b monsters other min-rem | Guardian naga Treasure line prints “5d6×1cp” — a bare multiplier of 1 with the coin abbreviation closed up — where the same line prints five correctly-formed values (1d%×1,000 sp, 10d4×1,000 ep, 10d6×1,000 gp, 5d10×100 pp). The form occurs exactly once in the book. |
| E253 | 298 | 310 | 23b monsters other min-rem | Water naga prose prints a three-item list with no commas at all: “fresh water lakes ponds and rivers”. |
| E254 | 299 | 311 | 23b monsters other min-rem | Night Hag prose prints a space after the mid-line hyphen in “fire- based”, where “cold-” earlier in the same phrase is a true suspended hyphen. “fire-” and “based” are separate word boxes at a 1.40 pt gap, matching every other word gap on the justified line. Same class as errata E45. |
| E255 | 300 | 312 | 23b monsters other min-rem | Nightmare stat block prints “Very Rare” with a capital R where the Nilbog stat block directly below on the same page prints “Very rare”. |
| E256 | 300 | 312 | 23b monsters other min-rem | Nilbog Treasure line prints the bold-italic run-in label “Treasure” with no colon, followed by an en space, where the label carries a colon at 311 other in-body sites. |
| E257 | 304 | 316 | 23b monsters other min-rem | Pseudo-Dragon prose prints “can be be found” — the verb doubled. |
| E258 | 305 | 317 | 24 monsters other roc-z | Roc, Treasure line: `1d33 jewellery (20%)` — an impossible die expression where `1d3` belongs; the same line prints `1d6 gems (25%)` correctly and the parallel Sea Hag line on book p.309 prints `1d3 jewellery (25%)`. |
| E259 | 308 | 320 | 24 monsters other roc-z | Sahuagin, Treasure line: `Individuals :1d6 pp each` — a word space before the colon and none after it; the same line sets `Treasure:` and `Lair: 2d6×1,000 gp` correctly. |
| E260 | 308 | 320 | 24 monsters other roc-z | Scorpion table, Special Defences row: `None-` with a trailing hyphen in all three variant cells, where the book sets `None` elsewhere and no continuation follows. |
| E261 | 308 | 320 | 24 monsters other roc-z | Sea Hag stat block: the label prints `MAGIC Resistance:` in full caps where every other label in the block, and the `Magic Resistance:` label in the Scorpion table 26 pt below on the same page, is Title Case. |
| E262 | 309 | 321 | 24 monsters other roc-z | Sea Hag, Treasure line: `go` for *gp*; the same line prints `cp` and `sp` correctly and the coin abbreviation appears nowhere else in the book as `go`. |
| E263 | 312 | 324 | 24 monsters other roc-z | Snake, Giant table, Special Defences row: `None-` with a trailing hyphen in all four variant cells, with no continuation. |
| E264 | 312 | 324 | 24 monsters other roc-z | Snake, Giant / *Boas*: `creatures creatures` — the noun printed twice. |
| E265 | 312 | 324 | 24 monsters other roc-z | Sphinx, Andro-: `with a  human torso` — a printed mid-sentence double space between plain words. |
| E266 | 312 | 324 | 24 monsters other roc-z | Sphinx, Andro-: `their female  counterparts,` — a printed mid-sentence double space between plain words. |
| E267 | 312 | 324 | 24 monsters other roc-z | Sphinx, Andro-: `will often  grant access` — a printed mid-sentence double space between plain words. |
| E268 | 312 | 324 | 24 monsters other roc-z | Sphinx, Andro-: `they are watching  (providing` — a printed mid-sentence double space between plain words. |
| E269 | 313 | 325 | 24 monsters other roc-z | Sphinx, Andro-: `endanger the  Androsphinx` — a printed mid-sentence double space between plain words. |
| E270 | 313 | 325 | 24 monsters other roc-z | Sphinx, Andro-: `payment  must be made in full` — a printed mid-sentence double space between plain words. |
| E271 | 313 | 325 | 24 monsters other roc-z | Sphinx, Andro-: `their would-be  employers` — a printed mid-sentence double space between plain words. |
| E272 | 313 | 325 | 24 monsters other roc-z | Sphinx, Andro-: `a deafening roar that  functions` — a printed mid-sentence double space between plain words. |
| E273 | 313 | 325 | 24 monsters other roc-z | Sphinx, Gyno- prose (printed in book p.313 col 1 under the Sphinx, Crio- stat block): `their kind prefers  riddles` — a printed mid-sentence double space between plain words. |
| E274 | 313 | 325 | 24 monsters other roc-z | Sphinx, Gyno- prose: `some sort of  payment for release` — a printed mid-sentence double space between plain words. |
| E275 | 313 | 325 | 24 monsters other roc-z | Sphinx, Gyno- prose: `a game of chess,  etc.).` — a printed mid-sentence double space between plain words. |
| E276 | 313 | 325 | 24 monsters other roc-z | Sphinx, Crio- prose: `with front  claws` — a printed mid-sentence double space between plain words. |
| E277 | 313 | 325 | 24 monsters other roc-z | Sphinx, Gyno- stat block: `Hit Dice :` with a word space before the colon; the Sphinx, Crio- block in column 1 of the same page prints `Hit Dice:` closed up, as does `Armour Class:` directly above it. |
| E278 | 314 | 326 | 24 monsters other roc-z | Spider, Giant stat block: `HIT DICE :` — full caps *and* a word space before the colon, where the same page sets `Hit Dice:` correctly three times and `Armour Class:` directly above is Title Case. |
| E279 | 314 | 326 | 24 monsters other roc-z | Spider, Giant: `their common,  tiny cousins` — a printed mid-sentence double space between plain words. |
| E280 | 314 | 326 | 24 monsters other roc-z | Spider, Huge: `saving throws made  against it are at +3` — a printed mid-sentence double space between plain words. |
| E281 | 314 | 326 | 24 monsters other roc-z | Spider, Large: `saving throws made  against it are at +2` — a printed mid-sentence double space between plain words. |
| E282 | 315 | 327 | 24 monsters other roc-z | Spider, Phase: `the phase spider  must remain in phase` — a printed mid-sentence double space between plain words. |
| E283 | 315 | 327 | 24 monsters other roc-z | Spider, Phase: `æthereal through magic  or other means` — a printed mid-sentence double space between plain words. |
| E284 | 315 | 327 | 24 monsters other roc-z | Spider, Phase: `they may  strike at it` — a printed mid-sentence double space between plain words. |
| E285 | 315 | 327 | 24 monsters other roc-z | Spider, Giant Water: `respects. They  differ in that` — a printed mid-sentence double space between plain words. |
| E286 | 315 | 327 | 24 monsters other roc-z | Spider, Giant Water: `they build  underwater lairs` — a printed mid-sentence double space between plain words. |
| E287 | 315 | 327 | 24 monsters other roc-z | Spider, Giant Water: `whereupon they will  scuttle out` — a printed mid-sentence double space between plain words, correctly reproduced in the file but never marked. The same paragraph carries three other double spaces, all three marked. |
| E288 | 315 | 327 | 24 monsters other roc-z | Spider, Giant Water: `poisoning them, cocooning them,  and removing` — a printed mid-sentence double space between plain words. |
| E289 | 316 | 328 | 24 monsters other roc-z | Stunjelly: `inflict upon a its prey` — a stray article before the possessive. |
| E290 | 318 | 330 | 24 monsters other roc-z | Triton lair composition: `60+ 1d6×-10 non-combatant children` — a minus sign before the multiplier and a space after `60+`, where the line immediately above prints `60+1d6×10 non-combatant females`. |
| E291 | 318 | 330 | 24 monsters other roc-z | Triton, Treasure line: five multipliers printed `×1000` with no thousands comma and closed up against the coin abbreviation (`1d12×1000cp`, `1d6×1000sp`, `1d4×1000ep`, `2d4×1000gp`, `1d6×1000pp`), where the book prints `×1,000` 437 times. |
| E292 | 319 | 331 | 24 monsters other roc-z | Wasp, Giant stat block: `Intelligence: Non` — a bare `Non` where the book's stat blocks print `Non-` (19 instances corpus-wide against two bare). |
| E293 | 319 | 331 | 24 monsters other roc-z | Will-O-the-Wisp, Treasure line: four multipliers printed `×1000` with no thousands comma, where the book prints `×1,000` 437 times. |
| E294 | 320 | 332 | 24 monsters other roc-z | Xorn, Treasure line: `2d6×1,000- gp` — a stray hyphen after the multiplier value; the three adjacent values on the same line print `1d4×1,000 cp`, `1d8×1,000 sp`, `1d2×1,000 ep` cleanly. |
| E295 | 321 | 333 | 25 treasure coin gems potions scrolls | COIN introduction: `heavy, and  weight is a significant drawback` — a printed mid-sentence double space between plain words. |
| E296 | 324 | 336 | 25 treasure coin gems potions scrolls | Rings Table 1: Properties, row 13 prints `01-25 Regeneration` then `25-00 Spell Storing` — the value 25 is in both sub-ranges. Row 16 three rows below prints `01-50` / `51-00`, continuous. |
| E297 | 326 | 338 | 25 treasure coin gems potions scrolls | Table II footnote ¹ mixes numeral systems in one enumeration: a roman `I` then an arabic `2`. Footnote ² 18 pt below on the same page prints `1 = Type I, 2 = Type II, 3 = Type III, 4 = Type IV`, roman throughout. |
| E298 | 327 | 339 | 25 treasure coin gems potions scrolls | Table IV: Rare Miscellaneous Magic Items: the roll range `41-32` runs backwards; every other range in the table ascends. |
| E299 | 328 | 340 | 25 treasure coin gems potions scrolls | Table IV: Rare Miscellaneous Magic Items, Sagacious Volume Value cell prints `50,000312` — a malformed number; the row above prints `75,000`. |
| E300 | 329 | 341 | 25 treasure coin gems potions scrolls | Potion Admixture Results Table, row 01: `with` where *within* belongs; the next printed line of the same cell reads `all persons within 10 ft of the epicentre`. |
| E301 | 330 | 342 | 25 treasure coin gems potions scrolls | Potion of Gaseous Form: `lightening` for *lightning*. |
| E302 | 332 | 344 | 25 treasure coin gems potions scrolls | Potion of Undead Control: noun `affects` where *effects* belongs; the very next printed line of the same paragraph uses the verb correctly — `affects one type of undead`. |
| E303 | 337 | 349 | 26 rods staves wands armour swords | Wand of Lightning: the body prints `wand of lighting` where its own bold entry name reads `Lightning (DM):` and the same entry three lines below prints `A wand of lightning can be recharged.` |
| E304 | 337 | 349 | 26 rods staves wands armour swords | Wand of Negation: the body calls the item a `rod` where the entry sits in the WANDS section and its name is `Negation (CDIM)`. |
| E305 | 338 | 350 | 26 rods staves wands armour swords | Wand of Wonder table, row 11–15: `the rod` where the table is a wand's; the same row's neighbours all say *wand*. |
| E306 | 338 | 350 | 26 rods staves wands armour swords | Wand of Wonder table: the `54-58` row uses an ASCII hyphen where the other 22 rows of the same table use en-dashes. |
| E307 | 338 | 350 | 26 rods staves wands armour swords | Plate Mail of Æthereality: `everything non-living thing` — three separate word boxes; reads as *every* plus a stray *thing*. |
| E308 | 338 | 350 | 26 rods staves wands armour swords | Plate Mail of Æthereality: the body prints `plate mail of ætherealiality` where the entry name three lines above reads `Plate Mail of Æthereality (CFPR)`. |
| E309 | 339 | 351 | 26 rods staves wands armour swords | Bleeding Sword: a verb is omitted after `this` — `whether this a natural ability`. |
| E310 | 340 | 352 | 26 rods staves wands armour swords | Holy Sword: `+ 2` with a full word space inside the bonus, where the same entry prints `+5`, `+10` and `50%` closed up. |
| E311 | 340 | 352 | 26 rods staves wands armour swords | Magebane: `does not qualify as  magic-using.` — a printed mid-sentence double space between plain words. |
| E312 | 340 | 352 | 26 rods staves wands armour swords | UNUSUAL SWORDS introduction: `self- aware` — a printed hyphen mid-line with a genuine word space after it, the line continuing past it. |
| E313 | 341 | 353 | 26 rods staves wands armour swords | Sword Major Powers, Speech: the paragraph ends `according to the table below` with no terminal full stop. |
| E314 | 341 | 353 | 26 rods staves wands armour swords | Note under Sword Alignment: a stray or misplaced `as` — `neutral-aligned as swords`. |
| E315 | 341 | 353 | 26 rods staves wands armour swords | Sword Minor Powers table, row 45-55: `detect traps 10 ft within radius` — word order reversed against nine parallel rows in the same table, all of which read `... within N ft radius`. |
| E316 | 342 | 354 | 26 rods staves wands armour swords | Special Purpose Swords footnote: ends `beings of extreme alignments` with no terminal full stop. |
| E317 | 344 | 356 | 26 rods staves wands armour swords | Holy Mace: `as the wielder were` — *if* is absent. |
| E318 | 344 | 356 | 27 miscellaneous magic a-gog | Alchemy Jug: `when poured. The  type and quantity of liquid` — a printed mid-sentence double space between plain words. |
| E319 | 344 | 356 | 27 miscellaneous magic a-gog | Amulet of Life Protection: `broach` for *brooch*; the book sets `Brooch of Shielding` and `Brooch of Instigation` correctly on book p.347. |
| E320 | 345 | 357 | 27 miscellaneous magic a-gog | Apparatus of the Lobster: `each of which controlling` — a participle where a finite verb belongs. |
| E321 | 345 | 357 | 27 miscellaneous magic a-gog | Bag of Holding: a bare printed mid-sentence hyphen in `type-listed`, with the line continuing past it. |
| E322 | 346 | 358 | 27 miscellaneous magic a-gog | Boots of Striding and Springing: `increases the wearer’s base speed  to 120 ft` — a printed mid-sentence double space between plain words. |
| E323 | 347 | 359 | 27 miscellaneous magic a-gog | Brooch of Instigation: noun `affect` where *effect* belongs; one sentence later the same entry prints `This boast is a mental effect much like *ESP*`. |
| E324 | 347 | 359 | 27 miscellaneous magic a-gog | Candle of Invocation: a bare printed mid-sentence hyphen in `flame-this`, where a dash or full stop belongs; the line continues past it. |
| E325 | 348 | 360 | 27 miscellaneous magic a-gog | Circlet of Persuasion: `by+3` closed up, with no space between the preposition and the bonus. |
| E326 | 349 | 361 | 27 miscellaneous magic a-gog | Cube of Frost Resistance: `creases` for *creates*. |
| E327 | 351 | 363 | 27 miscellaneous magic a-gog | Dust of Dryness: noun `affect` where *effect* belongs; the same sentence uses the verb correctly six words earlier — `will only affect water`. |
| E328 | 351 | 363 | 27 miscellaneous magic a-gog | Dust of Tracelessness: `allow` where *allowing* belongs. |
| E329 | 353 | 365 | 27 miscellaneous magic a-gog | Figurines of Wondrous Power, *Silver Raven*: `it` where the possessive *its* belongs. |
| E330 | 353 | 365 | 27 miscellaneous magic a-gog | Gem of Brightness, Light power: a word space before the comma — `30 ft radius , requires`. |
| E331 | 353 | 365 | 27 miscellaneous magic a-gog | Gem of Seeing: `May be used no more than  30 minutes per day.` — a printed mid-sentence double space between plain words. |
| E332 | 355 | 367 | 28 miscellaneous magic gog-z | *Iron Bands of Binding* entry heading prints a **space before the colon** — `Iron Bands of Binding (any) :`. The colon is its own word box at x 305.23–308.40, separated from `(any)` (ends x 303.77) by 1.46 pt, byte-for-byte the same gap as every other word space on the heading line (Iron→Bands, Bands→of, of→Binding, Binding→(any), all 1.46 pt). Same class as E18. The file's colonless `### Name` heading style cannot represent it, so the marker stands alone as an annotation rather than sitting after the text. |
| E333 | 356 | 368 | 28 miscellaneous magic gog-z | *Marvellous Pigments*: `will be only be` — **`be` duplicated**. The sentence reads correctly with either one of the two removed; nothing else on the page repeats a verb this way. |
| E334 | 356 | 368 | 28 miscellaneous magic gog-z | *Medallion of Thoughts*: `2nd  level` — a **mid-sentence double space**, gap 3.330 pt against a 1.672 pt line median, **1.99×**. E29-E57 class. |
| E335 | 357 | 369 | 28 miscellaneous magic gog-z | *Mirror of Life Trapping*: `may  be` — a **mid-sentence double space**, gap 2.287 pt against a 1.110 pt line median, **2.06×**. |
| E336 | 358 | 370 | 28 miscellaneous magic gog-z | *Ring Gates*: `of  material` — a **mid-sentence double space**, gap 2.227 pt against a **uniform** 1.058 pt for all thirteen other gaps on the justified line, **2.10×**. The word breaks over the line as `ma-`/`terial` (soft hyphen U+00AD, not a printed hyphen), so the wide gap is the last gap on the line but is not a sentence or label gap. |
| E337 | 359 | 371 | 28 miscellaneous magic gog-z | *Robe of Useful Items*: `2 of each of following items` — **`the` absent** after the second `of`. E24/E55 class. |
| E338 | 359 | 371 | 28 miscellaneous magic gog-z | *Robe of Useful Items* additional-patches d% table: the sequence runs `17 Bonfire` then `19-21 Cask` — **roll 18 is unassigned**, and the token `18` appears nowhere on book p.359. Every other row in the table is contiguous and the table otherwise runs 01 to 00. E4/E5 class. |
| E339 | 361 | 373 | 28 miscellaneous magic gog-z | *Greater Strand of Prayer Beads*: the bead name **`summons` prints with a roman initial `s` on an otherwise italic word** — the page's text layer splits it as `MyriadPro-SemiCn ', s'` + `MyriadPro-SemiCnIt 'ummons'`, while all three other occurrences of *summons* on the same page are wholly italic and the entry's styling is uniform across seventeen bead-name instances. SETTLED by audit batch 9's tie-breaker: the disputed `s` is bit-for-bit identical to 144/144 roman controls and 0/31 italic across four renderer x dpi combinations; the two CFF charstrings differ (DTMLDZ+MyriadPro-SemiCn ItalicAngle 0 vs CKCIHQ+MyriadPro-SemiCnIt at -11). E51 class. |
| E340 | 361 | 373 | 28 miscellaneous magic gog-z | *Sustaining Spoon*: `can produced` — **`be` absent**. Same class as E55 (`will also reduced by half`). |
| E341 | 362 | 374 | 29a rings and cursed items i | *Ring of Charisma*: `21 levels/hit dice **or** humans or humanoids` — **`or` where `of` belongs**. The sentence as printed offers a choice between a level total and a category of creature, which is not a construction the rule can bear; the parallel *charm person* wording elsewhere quantifies levels **of** targets. The same sentence's own second `or` (`humans or humanoids`) is correct, which is what makes the first legible as a slip. |
| E342 | 364 | 376 | 29a rings and cursed items i | *Ring of Wizardry* d% table, row 96-99: `1st , 2nd, and 3rd level` — a **space before the comma**. The comma is its own word box (x 247.8) preceded by a 1.058 pt gap against line word-spaces of 1.057-1.058 pt, i.e. exactly one word space. The two adjacent commas in the same cell are set closed up. Same class as E18 and as the `Light: 30 ft radius ,` site in file 27. |
| E343 | 364 | 376 | 29a rings and cursed items i | CURSED ITEMS introduction: `The listing … **provide** some examples` — **singular subject, plural verb**. The head noun is `The listing`; `items` is inside a prepositional phrase. |
| E344 | 365 | 377 | 29a rings and cursed items i | Drawback d% table, row 21-25: `begins **glowing the dark**` — **a preposition is absent** (`in the dark`). Read at 1200 dpi: no clipped glyph, normal word gaps, nothing overset at the line break. |
| E345 | 367 | 379 | 29a rings and cursed items i | *Boots of Dancing*: `8th  magic` — a **mid-sentence double space**, gap 3.292 pt against a 1.650 pt line median, **2.00×**. |
| E346 | 367 | 379 | 29a rings and cursed items i | *Boots of Dancing*: `the 8th  magic user spell` is **missing the word `level`**, and the surplus space sits exactly where it would go. Every parallel construction in book pp.362-368 prints it: `3rd level magic user spell`, `1st level`, `2nd level` (book p.362), `5th level`, `9th level`, `7th level` (book p.364), `1st level druid spell` (book p.368) — seven for seven. A **second, distinct fault at a site the file already marks for its double space**. |
| E347 | 368 | 380 | 29b cursed items ii and artifacts | *Periapt of Foul Rotting*: `by a application of a` — **`a` before a vowel**. Identical class to E47 (`an non-tool-using creature`), inverted. |
| E348 | 369 | 381 | 29b cursed items ii and artifacts | *Stone of Weight, or, Loadstone*: `A egg-shaped` — **`A` before a vowel**. E47 class. |
| E349 | 369 | 381 | 29b cursed items ii and artifacts | *Stone of Weight, or, Loadstone*: **`lapus lazuli`** for *lapis lazuli*. The book sets the mineral correctly as `lapis lazuli` at book p.322 (gem-value table) and book p.347; this is the only `lapus` in the volume. E14 class (a single-letter slip with in-book controls). |
| E350 | 370 | 382 | 29b cursed items ii and artifacts | *Sword of the Berserker +2*: `no living creatures is` — **plural subject, singular verb**. E26/E27 class. |
| E351 | 370 | 382 | 29b cursed items ii and artifacts | ARTIFACTS introduction: `other-planar  influences` — a **mid-sentence double space**, gap 2.025 pt against a 0.938 pt line median, **2.16×**. The widest ratio in the group. |
| E352 | 370 | 382 | 29b cursed items ii and artifacts | *Book of Infinite Spells* spell-level table: the right-hand block prints `86–95` then `95–00` — **the boundary value 95 falls in both rows**. Identical class to E6 and E7 (04 and 13 duplicated in the Table IV roll ranges). |
| E353 | 371 | 383 | 29b cursed items ii and artifacts | *Deck of Many Things*, **Gem**: `and  worth` — a **mid-sentence double space**, gap 2.715 pt against a 1.320 pt line median, **2.06×**. |
| E354 | 371 | 383 | 29b cursed items ii and artifacts | *Deck of Many Things*, **Jester**: `discarded  before` — a **mid-sentence double space**, gap 2.715 pt against a 1.320 pt line median, **2.06×**. |
| E355 | 371 | 383 | 29b cursed items ii and artifacts | *Deck of Many Things*, **Knight**: `the  character.` — a **mid-sentence double space**, gap 2.242 pt against a 1.076 pt line median, **2.08×**. Control on the same page: `the character.` at y 461.1 measures 1.200 pt against a 1.200 pt median, **1.00×**, and is correctly unmarked. |
| E356 | 371 | 383 | 29b cursed items ii and artifacts | *Deck of Many Things*, **Rogue**: `religious  figure,` — a **mid-sentence double space**, gap 2.085 pt against a 0.975 pt line median, **2.14×**. |
| E357 | 371 | 383 | 29b cursed items ii and artifacts | *Deck of Many Things*, **Skull**: `a  fight` — a **mid-sentence double space**, gap 3.383 pt against a 1.702 pt line median, **1.99×**. |
| E358 | 373 | 385 | 29b cursed items ii and artifacts | *Hammer of Thunderbolts*: `the hurled weapons emits` — **plural subject, singular verb**. E26/E27 class; same fault as the *Sword of the Berserker* site three pages earlier. |
| E359 | 373 | 385 | 29b cursed items ii and artifacts | *Philosopher's Stone*: `one must decided` — **past participle for infinitive** after a modal. E44 class (`will negates`). |
| E360 | 373 | 385 | 29b cursed items ii and artifacts | *Talisman of Pure Good*: `cleric  (LE,` — a **mid-sentence double space**, gap 3.150 pt against a 1.560 pt line median, **2.02×**. Not a post-label gap: `cleric` is a plain word, not a run-in label. |
| E361 | 381 | 393 | 30 compiled tables | Appendix A **Magic User To Hit** table span caption prints `Roll required to hit Armour Class` in **mixed case**. Census of all nine such captions in Appendix A (book pp.375-388): eight are set `ROLL REQUIRED TO HIT ARMOUR CLASS` in full caps (book pp.376, 377, 378, 379, 380, 383 x2, 385) and this one alone is mixed case. Same class as E28, which records the identical fault in the Chapter I Magic User table at book p.19 — **a distinct second location, not a duplicate**. |
| E362 | 384 | 396 | 30 compiled tables | Table caption prints `Thief Skills Table—Base chance` — **lower-case second word**. The third caption in the same set on the same page reads `Thief Skills Table—Racial Adjustments` in Title Case, which is what makes it legible as an inconsistency. |
| E363 | 384 | 396 | 30 compiled tables | Table caption prints `Thief Skills Table—Dexterity adjustments` — **lower-case second word**, against `…—Racial Adjustments` on the same page. Distinct from the `Base chance` caption above and separately marked, as E26/E27 are. |
| E364 | 386 | 398 | 30 compiled tables | **Melee Weapon Table** column header prints `Weapon type` — **lower-case `t`** — while the **Missile Weapon Table lower on the same page** prints `Weapon Type`, and its continuation on book p.387 does too. Its own neighbouring headers (`Damage vs Small or Medium`, `Damage vs Large`, `Encumbrance`, `Cost`) are all Title Case. |
| ~~E365~~ | 387 | 399 | 30 compiled tables | **RETRACTED 2026-09-07 by the owner. E365 was wrong — the closed-up `1gp` is NOT an error, and the in-file marker has been removed from file 30. Do not re-mark it.** It read: *"Appendix A Missile Weapon Table, Hammer row: the Cost cell prints `1gp` closed up where Javelin (`5 sp`), Sling (`5 sp`) and Spear (`1 gp`) in the same table print two boxes with a space."* That reading of the page is accurate and was re-confirmed at 1200 dpi and at word-box level — Hammer's cost is a single box at x 364.6 against two boxes each for the three rows below, and it is the only closed-up value among 54 coin values on book pp.386–387. **But the leave-alone list already ruled the identical cell on book p.33 to be house style, and a SECOND independent table reprinting the same closed-up cell makes deliberate typesetting more plausible, not less.** The ruling widened the leave-alone note to name book p.387 as well as p.33, rather than promoting either. **Retracted, not deleted, so a future pass reading file 30 against the register does not find a silent gap and re-derive the same wrong conclusion.** File 30 transcribes the cell as `1gp`, exactly as printed, and is correct as delivered. |
| E366 | 393 | 405 | 32 index | INDEX, *Ability Scores*: `34,51,` — **no space after the comma**, where every other separator in the same page list has one. The two numbers extract as a single word box. |
| E367 | 393 | 405 | 32 index | INDEX, *Alignment*: `ix,  4,` — a **double space inside the page list**, 2.041 pt against a 1.021 pt line median, **ratio exactly 2.00**. |
| E368 | 393 | 405 | 32 index | INDEX, *Attribute (Ability Score)*: the record ends `249,` — a **dangling trailing comma** with nothing after it. One of five in the general index. |
| E369 | 393 | 405 | 32 index | INDEX, *Character*: the record ends `ix,` — a **dangling trailing comma**. |
| E370 | 393 | 405 | 32 index | INDEX, *Cleric*: `3,  10-12,` — a **double space inside the page list**, 2.041 pt against a 1.020 pt line median, **ratio exactly 2.00**. |
| E371 | 393 | 405 | 32 index | INDEX, *Demi-Humans*: `141,142,` — **no space after the comma**; the pair extracts as a single word box. |
| E372 | 393 | 405 | 32 index | INDEX, *Die, Dice, “D”*: the record ends `ix,` — a **dangling trailing comma**. |
| E373 | 393 | 405 | 32 index | INDEX, *Elves (Elf, Elvish)*: `3-5 , 51,` — a **space before the comma**. The comma is its own word box at x 222.1 preceded by a 1.020 pt gap, exactly the line's word-space median. Same class as E18. |
| E374 | 393 | 405 | 32 index | INDEX, *Exploring the Planes*: `iii,  152` — a **double space inside the page list**, 2.041 pt against the page's 1.020-1.027 pt word-space median, **ratio 2.00**. The record has only one internal gap, so the control is the page median rather than a line median. |
| E375 | 393 | 405 | 32 index | INDEX, *Hit Points (HP)*: the record ends `145,192` — **no space after the comma**; the pair extracts as a single word box. |
| E376 | 394 | 406 | 32 index | INDEX, *Scrolls, Read*: the record ends `25,` — a **dangling trailing comma**. |
| E377 | 394 | 406 | 32 index | INDEX, *Spells, Druid*: the **whole record is set bold** (`MyriadPro-SemiboldCond` for the page list as well as the headword, where every other record sets the list in `MyriadPro-Cond` regular) and an **en dash stands where the U+2002 en-space separator belongs**. Its two siblings *Spells, Cleric* and *Spells, Illusionist* are set normally on the same page. Audit batch 9 established what these two anomalies actually are: the **only two of the book's 42 no-en-space records that carry page numbers**. |
| E378 | 394 | 406 | 32 index | INDEX, *System Shock*: the **whole record is set bold** and it opens with a bare **`-2`** — an ASCII hyphen standing where the en-space separator belongs, so the record reads as if the first page number were minus two. Sibling to the *Spells, Druid* anomaly above; the second of the two no-en-space records carrying page numbers. Note the two use different dashes: `–` there, `-` here. |
| E379 | 394 | 406 | 32 index | INDEX, *Tracking*: the record ends `23,` — a **dangling trailing comma**. Fifth and last of the class in the general index. |
| E380 | 395 | 407 | 32 index | INDEX OF TABLES, *Character Class > Ranger > Saving Throw*: `23 24, 370` — **the comma between 23 and 24 is absent**; the gap measures 1.021 pt against a 1.021 pt line median, i.e. one ordinary word space. The other eight Saving Throw records and all nine To Hit records in the *Character Class* group comma-separate their page numbers. |
| E381 | 395 | 407 | 32 index | INDEX OF TABLES, *Character Class > Ranger > Saving Throw*: cites **page 370** for the *Ranger Saving Throw Table*, which is printed on book **p.385**; book p.370 is cursed-swords prose. Identical in kind to F1 on the very next line, and like F1 it does **not** fit the +12 signature (370+12 = 382, not 385). Every sibling in the group cites its Appendix A page second — Cleric 376, Druid 377, Fighter 378, Illusionist 379, Magic User 381, Paladin 382, Thief 383 — and the book's own general index gives `Ranger iii, 22-24, 385`. |
| E382 | 395 | 407 | 32 index | INDEX OF TABLES, *Character Class > Ranger > To Hit*: cites **page 370** for the *Ranger To Hit Table*, which is printed on book **p.385**; book p.370 is cursed-swords prose and carries no table. **A defect class the project had not previously recorded: a wrong page NUMBER in an index, rather than a wrong word.** Corroborated by the book's own general index (`Ranger iii, 22-24, 385`) and by every sibling in the group giving its Appendix A page second (Paladin 383, Thief 383, Magic User 381). Unlike the three *Treasure > Weapons* entries below, this does **not** fit the +12 compositor signature (370+12 = 382, not 385). Audit batch 9 fix F1. |
| E383 | 395 | 407 | 32 index | INDEX OF TABLES, *Druid Spell > Confusion - Action*: a **plain hyphen** stands where the parallel records use an en dash. Measured from the embedded font: the glyph's advance is **1.813 pt** against **3.250 pt** for the 36 same-page en-dash controls; at 1200 dpi its ink width is 1.440 pt (24 px) against 2.880 pt (48 px), an **ink-width ratio of exactly 2.00**. Only three hyphens exist on book p.395: this, the *Men - (Leader Type)* record below, and the legitimate compound `On-Off`. |
| E384 | 395 | 407 | 32 index | INDEX OF TABLES, *Magic User Spell > Prismatic Sphere*: prints the gloss **lower-case, `(color)`**, where the adjacent *Prismatic Spray – Colour (Color)/Effect* record on the same page prints `(Color)`. The book preserves both `Colour (color)` and `Colour (Color)` and neither is to be harmonised; the marker records the inconsistency. |
| E385 | 395 | 407 | 32 index | INDEX OF TABLES, *Monsters > Men - (Leader Type) Magic Item*: a **plain hyphen** where the parallels use an en dash — including the sibling *Men – Pilgrim Alignment* eight lines below, which prints an en dash. Advance 1.814 pt against the page's 36 en dashes at 3.250 pt. Second of the two. |
| E386 | 396 | 408 | 32 index | INDEX OF TABLES, *Treasure > Potion > Giant Strength – Type/ Ability*: a **space after the slash**. Of the 21 slash-bearing records on book p.396 this is the **only** one so set; the rest (`Ioun Stones – Color/Shape/Effect`, `Cube of Force – Attack Type/Charges`, `Strand of Prayer Beads – Type/Ability`, `Necklace of Fireballs – Type/Number` and the rest) close the slash up. Same class as the printed `Open Locks/ Disarm Traps:` recorded in the leave-alone list for book p.25. |
| E387 | 396 | 408 | 32 index | INDEX OF TABLES, *Treasure > Weapons > Special Magical Miscellaneous*: cites **page 313** for the *Special Magic Miscellaneous Weapons* table, which is printed on book **p.325**; book p.313 is the Androsphinx monster entry. **A wrong page NUMBER in an index — a defect class the project had not previously recorded.** The offset is exactly **+12**, the arabic-zone book-to-PDF offset: **the compositor appears to have used PDF page numbers rather than printed folios**. Audit batch 9 fix F4. |
| E388 | 396 | 408 | 32 index | INDEX OF TABLES, *Treasure > Weapons > Table 1: Form, Miscellaneous*: cites **page 311** for *Miscellaneous Weapons Table 1: Form*, printed on book **p.323**; book p.311 is the Skeleton Warrior monster entry. **+12 — a PDF page number printed as a folio.** Corroborated by the book's own general index, `Miscellaneous Weapons iv, vi, 323-325, 343`. Audit batch 9 fix F2. |
| E389 | 396 | 408 | 32 index | INDEX OF TABLES, *Treasure > Weapons > Table 2: Properties, Miscellaneous*: cites **page 312** for *Miscellaneous Weapons Table 2: Properties*, printed on book **p.324**; book p.312 is the Snake, Giant monster entry. **+12 — a PDF page number printed as a folio.** Audit batch 9 fix F3. |
| E390 | 126 | 138 | 12 time movement combat | DAMAGE AND DEATH, simultaneous initiative: `the effects of damage␣␣inflicted during that segment` — a printed mid-sentence double space, gap **2.7375 pt against a uniform 1.3125 pt** for all eight other word gaps on the same justified line (2.09×). The control is on the same page and in the same column, exactly 45.0 pt above: `The damage inflicted by combatants` prints the identical bigram at **1.0050 pt**. **The delivered file had normalised the space away, which is why this site could not be given an ID in the 2026-09-07 errata pass — marking normalised text `printed as-is` would have been a false claim. The space was restored on 2026-09-07 and the marker added in the same edit.** |
| E391 | viii / 364 | 10 / 376 | 01 lists (the omission) / 29a rings and cursed items i (the entry) | **A THIRD entry that the book's own List of Magic Items omits while printing it in full in the body — the same fault as E60, found on 2026-09-07 and unrecorded before.** *Ring of Telekinesis* is printed and fully described on book p.364, with its complete *Maximum weight in lbs* d% table, between *Ring of Swimming* and *Ring of Three Wishes*. The front-matter RINGS block on book p.viii runs **fifteen rows** — Charisma, Feather Falling, Fire Resistance, Free Action, Genie Summoning, Invisibility, Protection, Regeneration, Spell Storing, Spell Turning, Swimming, Three Wishes, Warmth, Water Walking, Wizardry — with *Swimming* directly adjacent to *Three Wishes*: the slot is not merely unfilled, the neighbours abut. Confirmed independently at 900 dpi from both sides by two agents. The book's own back index carries the entry (see E392). **File 01 is not at fault** — it transcribes the list exactly as printed, including the omission — and file 29a carries the entry, which is why its roster comes to 33 against the list's 32. **Do not add the missing entry to file 01.** |
| E392 | 396 | 408 | 32 index | INDEX OF TABLES, *Treasure > Ring > Ring of Telekinesis – Maximum Weight*: cites **page 363** for the *Maximum weight in lbs* table, which is printed on book **p.364** as part of the *Ring of Telekinesis* entry. Read at 900 dpi, folio at 1200 dpi. **A sixth wrong page number in this index, and unlike E387–E389 it does not carry the +12 signature** — it is off by one, on its own. Both neighbours are correct (`of Spell Turning – Result 363`, table on p.363; `of Wizardry – Level(s) Doubled 364`, table on p.364), so this is not a systematic shift. Found on 2026-09-07 by an agent checking something else — **the second of these found that way, so the set is not demonstrably closed at six.** |
| E393 | 62 | 74 | 07 spells druid | Fire Storm stat block prints `Area of effect:` with a **lower-case `e`**, where the same page prints `Area of Effect:` five times and the rest of the file 77 times. Span font `MyriadPro-SemiboldSemiCn` 7.5 pt, confirmed at 1200 dpi — the label is genuinely printed that way, not an extraction artefact. **The only instance in the whole six-file spells set.** Same class as E28 and E362/E363, a label in the wrong case. Found on 2026-09-07 during the file 07 stat-line normalisation. |

Sixty assigned IDs — fifty-nine standing, one (E16) retracted, all confirmed by rasterising and reading the
page. E1 alone covers ten separate instances. Not claimed exhaustive
— more will surface during transcription, and this file gets appended
to as they do. E17 to E20 are proof of that. All four were found by transcribers, not
by recon — a wrong-but-plausible page number, a stray space before a
full stop, and two single-letter slips inside repeated boilerplate
break no pattern a script can test. E24 to E29 are more of the same, all
six found by batch 2 transcribers: dropped words, a singular for a
plural, a stray hyphen, a label in the wrong case. Every one reads
perfectly well until set beside its own parallel elsewhere in the book,
which is how each was actually caught — by census against the other ten
class tables, the other race entries, the other credit lines. That is
the method that works on this book, and it is not scriptable. Expect
more.

**UPDATE — 2026-09-07, the errata maintenance pass. The register now stands at
393 assigned IDs: 391 standing, two (E16 and E365) retracted.** E390–E393 were
added later the same day by the repair pass that followed, and are described
at the end of this note. The paragraph above
describes the state at sixty IDs and is left as written. **E61 to E389 are
additive; nothing above them was revised, narrowed or rescoped, and no
leave-alone ruling was touched.**

**What E61–E389 are.** 329 printed defects across 30 files, every one of them
already found, verified against the page image and reproduced verbatim in the
delivered text by an earlier pass — this pass assigned the IDs and did not
discover the defects. **261 of them already carried an in-file
`<!-- printed as-is: NEW -->` marker** and were relabelled by scripted
find-and-replace; **68 carried no marker at all** and had one inserted at the
site. **IDs run in corpus order** — manifest file order, then line order, then
left-to-right within a line — so the block reads in book order rather than in
the order the defects were found.

**Containment.** The pass changed HTML comments and nothing else: **strip every
HTML comment from all 42 delivered files and the pre-pass and post-pass
corpora are byte-identical**, line counts unchanged, the 66 pre-existing
`see errata E1`–`E60` references untouched, zero `NEW` markers remaining, and
E61–E389 each present exactly once. Every pre-existing reference below E61
survives with unchanged multiplicity — matching `errata E<n>` anywhere in the
corpus gives **70 occurrences across 55 distinct IDs**, identical before and
after. (An independent verifier counting only the canonical
`printed as-is: see errata E<n>` form gets 68; the two figures differ by two
references worded inside a longer comment, and both are unchanged by the pass.)

**The class distribution, which is the useful part.** The largest single class
is the **printed mid-sentence double space at 71 entries** — over a fifth of the
block, and the only class on this project that is reliably scriptable, by
measuring each mid-line gap against its own line's median. Everything else is
long-tailed: punctuation 25, wrong word 23, spacing 19, inconsistency 18,
omitted word 16, dropped word 11, and then 51 further classes — 63 in all — with
five members or fewer. **That shape is the argument for the census method the register has
used since E30: the double spaces were found by measurement and the rest were
found by parallel-reading, and neither instrument finds the other's defects.**

**Five entries are a defect class the project had not seen before this pass:
wrong page NUMBERS in an index** — **E381, E382, E387, E388 and E389**, all in
file 32. **Three** of them carry the **+12 signature** — the arabic page offset — i.e. the compositor
appears to have used PDF page numbers where printed folios belong. An index is
the one file in the book where a page number can be checked against the thing it
points at; **in every other file a transposed number is invisible.** Whether the
front-matter lists on book pp.iv–viii carry the same fault is **still untested**.

**One recorded defect was deliberately NOT given an ID**, and it is the one to
read: book p.126 (file 12) prints `the effects of damage␣␣inflicted during that
segment` — a genuine mid-sentence double space, 2.74 pt against a uniform
1.31 pt line median, with a same-page control 45 pt above printing the identical
word pair at 1.005 pt. **The delivered file has normalised the space away**, so
marking it `printed as-is` would attach that claim to text that is not as
printed. It needs a transcription fix before it can carry an ID. **Flagged, not
resolved.**


E30 to E33 are different: printed mid-line double spaces, found not by
reading but by measurement — the batch-2 audit's word-box gap scans,
comparing each mid-line gap against its line's median. Three of the four
had been silently normalised to single spaces in transcription and were
restored from the page geometry. This class *is* scriptable — see the
wide-gap scan in `01 transcription template.md` — and the risk runs the
other way from every other entry in this table: not failing to spot
them, but normalising them away.

The scan has since been run over every delivered range and is standing
policy for new transcription. E34 to E37 came from the back-fill over
the batch-1 and batch-2 ranges; E38 to E57 from the batch-3
transcribers' own scans and parallel-reading. The mid-sentence
double-space class stands at **nineteen confirmed members** (E29's
second fault, E30–E37, E39, E41–E43, E50, E52–E54, E56–E57 — the
double-space items only), seven of them after the word `whether`
(E29, E33, E34, E39, E41, E42, E53). See
the sentence-spacing entry in the leave-alone list for what does NOT
qualify: only a mid-sentence wide gap between plain words is an
erratum.

---

## Ruled out — leave these alone

Every one of these looks like an error and is not. Do not correct them.
Do not log them.

**British spellings throughout.** *armour, defences, jewellery,
neutralise, manoeuvre, sceptre, meagre, marvellous, colouration,
valour.* House style, consistently applied. An American spellcheck
flags around ninety of these. None are errors. Note that E13
(`Labouratory`) is the one case where the house style was over-applied
and *is* an error — that is the exception, not a licence to hunt for
others.

**To-hit values of 21 to 26** in the class To Hit tables. Legitimate.
These are the rolls needed against AC −10 and below, and they are
correctly unachievable on a d20. Do not confuse these with E8, where an
*item saving throw* exceeds 20 — that table's own range tops out at 20.

**`51-00` → `01-50` sequences on pp.324–325.** False positives. These
pages carry many small independent d% sub-tables side by side; a scanner
reading in extraction order runs one sub-table's last row into the next
one's first. The tables themselves are continuous.

**`estab/lishes`, `comple/`, `cluding`, `vege/tarian`, `impri/soned`,
`ance`.** Hyphenated line breaks **in the extraction output**, not
printed text. De-hyphenate and rejoin as normal.

**This entry covers extraction artefacts only, and nothing else.** It
does **not** authorise removing a hyphen that is printed mid-line. The
test is position, not spelling: if the word sits at the end of an
extracted line and the remainder opens the next, it is an artefact and
you rejoin it; if text continues after it on the same printed line, the
hyphen is on the page and must be reproduced. `estab-lishes` on book
p.10 is exactly that second case and is logged as **E25** — it was
nearly suppressed under this entry, which is why the entry now says so.
Check the word-box geometry before invoking this ruling on any instance
not named above.

**`\t` at the head of extracted front-matter pages.** A byte-order mark
plus a real tab in the *extraction output*, produced by the running
head. **Not** the same thing as E1 and E2, which are printed glyphs on
the page. Anyone grepping for `\t` will hit both; only the p.398
instances are real.

Two corrections to this note, from the front-matter job. It is **not
limited to the verso pages 6, 8, 10, 12** — PDF 11 (recto) carries it
too, ordered the other way round (`ix\t` rather than `\tx`), because
recto and verso order the running-head elements differently. Do not
treat any page list as a whitelist. And using `-y 38`, the artefact
never appears at all: the crop starts below the running-head band. It
only shows up in uncropped extraction.

**`(AIMT):` on p.356.** An abbreviation, not a mangled word.

**`Homonculus`.** The book's spelling, seventeen occurrences, zero of
the conventional form. House style. Not an error.

**`Ioun Stones`.** A capital I, not a lowercase L. Confirmed at 600 dpi
and against the font's ToUnicode map.

**`L Shield +1, Missile Deflector` — SCOPED 2026-09-06. This applies to the
FRONT-MATTER LIST ON BOOK p.vii ONLY.** That page really does print a bare `L`
(its own 2.408 pt word box, x 216.108–218.516), confirmed at 600 dpi. **The body
entry on book p.339 prints the full word `Large`** (a single 17.3 pt box,
x 48.000–65.3025), also confirmed at 600 dpi. The book is inconsistent with
itself; see **E58**. This note originally named no page, which is why three
separate passes between batch 13 and audit batch 8 measured p.339, found
“Large”, and logged a conflict that never existed. **File 01 (`L Shield`) and
file 26 (`Large Shield`) are both correct. Never harmonise them, and never
“correct” either one to match the other.**

**Entries out of alphabetical order.** Scattered throughout all three
front-matter lists and, by extension, the chapters they index. Many
dozens of cases. The book's order is the order — never re-sort, and
never assume the next entry alphabetically is the next entry printed.

**`Dread Wraith` printed after `Yeti` in the List of Monsters, pointing
at page 372.** Out of sequence in both name and page number, and 372 is
in the artifacts range. Confirmed at 600 dpi. Reproduce as printed;
no explanation has been established.

**Inconsistent abbreviation and capitalisation between spell classes.**
The same spell is set differently in different class lists — differing
capitals, differing commas, differing abbreviations. Preserve each as
printed in its own list. Do not harmonise them.

**Non-ASCII glyphs.** Curly apostrophes, `æ`/`Æ`, and `ä` all appear as
genuine printed characters. Reproduce them; do not substitute ASCII.

**No en-dashes in the front-matter lists.** Every dash there is an ASCII
hyphen — verified by byte inspection. This does *not* generalise: the
p.107 table genuinely uses en-dashes. Check, don't assume, per range.

**US spellings that survive inside British-house-style text.** `color
application` in the p.ii credits, and `abridgment` in the OGL on p.398.
The book is otherwise consistently British. Reproduce as printed.

**`a traditional cube-shaped dice`** on p.ix — singular *dice*. Printed
that way. Possibly deliberate.

**`potation`, `creatures characters`, `Jonathon Jones`, and `Inc`
without a full stop throughout the p.398 credits.** All printed. All
confirmed at 600 dpi by the licence audit. Leave them.

**Wide gaps after a full stop.** The book's systematic sentence
spacing, not printed errors. File 05 established this: fifteen
instances on pp.36–37 alone, each at almost exactly 2× its line's
word-space median — a consistent typesetting behaviour, corroborated
by the 27 sentence/label gaps censused on pp.28–35 in batch 2. The
same census logic covers **wide gaps after bold run-in labels and
colons** (established on pp.8–17 and pp.28–35; applied to the p.55
Symbol sub-labels in batch 3). All are carried as single spaces in the
delivered files, matching every file shipped to date. **Only a
mid-sentence double space between plain words qualifies as an
erratum** — that is what the double-space items among E29–E57 are.
Do not log or carry a sentence-boundary or post-label wide gap.

**`the wilding power of illusion`** in the GNOMES entry on p.5.
Investigated at 600 dpi during the batch-2 audit: the glyphs are
confirmed, and no parallel passage elsewhere in the book makes it
legible as an error rather than a coinage. Possibly deliberate.
Reproduced as printed, no marker. Recorded here so nobody investigates
it twice.

**`"glibbering"` on p.247.** Printed inside quotation marks, which
suggests a deliberate coinage for a creature's noise rather than a slip
for "gibbering". Unverified visually. Leave it.

**The p.245 unicorn illustration.** By machine metrics this is the most
suspicious page in the book — 7,441 vector curves, hundreds of times any
other page. It is one finely-hatched decorative unicorn at the head of
the Undead chapter. Recorded here so nobody investigates it twice.

**`Treasure:` and `Description:` label styling — the book uses TWO forms
and they are semantically distinct. Settled 2026-09-06 by font census;
do not harmonise them.** Both are set in `MyriadPro-SemiboldSemiCn`, but
two embedded subsets are in play — `PZBCFL+…SemiboldSemiCnIt` (italic
flag set) and `XQBJRP+…SemiboldSemiCn` (upright). Measurably different:
"Treasure:" sets 26.8 pt italic against 27.6 pt upright.

- **Italic form → `***Treasure:***` / `***Description:***`.** Used for the
  prose Treasure and Description lines that follow a monster entry. This
  is the overwhelming majority — 308 instances across book pp.194–372.
- **Upright form → `**Treasure:**`.** Used for stat-block *row* labels
  (alongside `Frequency:`, `Hit Dice:`, `Alignment:`, which are all
  upright) and for the stat-block legend paragraph. Only **three**
  instances exist in the whole monster chapter: book p.193 once (the
  legend paragraph, "Treasure values are for the maximum possible
  number…") and book p.196 twice (`Treasure: See below` table rows). All
  three are in file 17a, which reproduces them correctly.

A blanket rule in either direction is wrong. **Reproduce whichever form
the page prints, checked by the italic flag on the span.** Note that the
bold-only "Treasure" appearing once per page from book p.322 onward is
the Chapter VI running head, not a label.

**The p.302 pegasus credit line.** The illustration carries
*(Illustration by Pearson Scott Foresman, http://commons.wikimedia.org)*
beneath it. This is the only in-body illustration credit in the book.
It is printed text and must be **transcribed**, not treated as an
artefact.

**"Damage vs Small or Medium / Damage vs Large" collapsing into one run
on p.387.** A `-layout` wrapping artefact of stacked header cells. The
page prints two distinct columns. Rasterise and reproduce the printed
structure.

**Field labels and styling in the Chapter I racial entries.** The seven
races on pp.3–7 label and style the same fields inconsistently, and all
of it is printed. Capitalisation varies (`Permitted class options:`
against `Permitted Class Options:`; `Multi-class Restrictions:` with a
capital R for half-orcs alone; a bare `Class Options:`). Hyphenation
varies (the heading `HALF ELVES` unhyphenated beside `HALF-ORCS`
hyphenated, with "half-elven" hyphenated in that same section's body).
Weight varies (the `Minimum/Maximum ability scores (after adjustment for
race);` line is regular weight for dwarfs and bold for the five other
races that carry it — confirmed from the embedded font names, not by
eye). Comma use varies (`Paladins, and Rangers` in two Constitution rows
against `Paladins and Rangers` in a third). Wording varies where the
sense is parallel (`Str 16 or less` for dwarfs against `Str 16 and
below` for elves and half-elves; the multi-class rule reading "the more
restrictive" for dwarfs, "the less restrictive" for elves).

These entries invite harmonisation more than anything else in the book,
because they are visibly a set and the variation looks like drift.
**Reproduce each race exactly as printed and never harmonise one against
another.** A transcription in which the seven races agree is a
transcription that has lost something.

**Coin values closed up in prose, spaced in tables.** The book writes
`1gp`, `75gp`, `30-180gp` closed up in running prose and `1 gp` spaced
inside tables. Both are house style, consistently applied in their own
contexts. Reproduce each as printed and do not impose one form on the
other. The single closed-up cell in the p.33 Missile Weapon Table — the
Hammer row's Cost, printed `1gp` where the same value is set `1 gp`
nineteen times across the six tables on pp.32–33 — is an inconsistency
inside a table that otherwise spaces every instance. It is reproduced as
printed and is **not** logged as a certain error, because the book's own
prose form makes it defensible. Left here rather than in the table above
deliberately: do not "fix" it, and do not promote it to an erratum
without new evidence.

**WIDENED 2026-09-07 by the owner: this ruling now names BOOK p.387 AS WELL
AS p.33.** Appendix A reprints the Missile Weapon Table at book p.387 and
prints the identical closed-up `1gp` in the same Hammer row — confirmed at
1200 dpi and at word-box level, Hammer's cost a single box at x 364.6
against two boxes each for Javelin, Sling and Spear, and the only closed-up
value among the 54 coin values on book pp.386–387. **A second independent
table repeating the same closed-up cell makes deliberate typesetting more
plausible, not less.** File 30 had marked the reprint as **E365**; that entry
is **retracted** and its in-file marker removed. Both instances are house
style: reproduce both as printed, correct neither, mark neither. **This note
originally named only p.33 — which is exactly the defect that made
`L Shield` cost five batches. A ruling that cites a reading must cite its
page, and now this one cites both.**

**Level Advancement footnotes and Thief Skills sub-labels in Chapter I.**
The per-class advancement footnote under the class level tables is set
four different ways across book pp.8–27, all printed:

- `Each level gained thereafter requires N experience points and grants
  +N hit point(s).` — pp.11, 17, 19
- `Each level gained thereafter requires N additional experience points
  and gains Nhp.` — pp.15, 21, 23
- `Each level thereafter requires N experience points and grants +2 hit
  points.` — p.26, dropping "gained"
- `*Level 15 at 1,500,000 experience points is the ceiling for
  assassins…` — p.9, a ceiling statement rather than a per-level one

So `experience points` against `additional experience points`, and
`grants +N hit point(s)` against `gains Nhp`, vary between classes that
otherwise read as a set.

The thief skill labels vary the same way between the descriptive section
on p.25 and the table on p.26 — `Climb:` against `Climb Walls`, and
`Open Locks/ Disarm Traps:` (with a printed space after the slash)
against `Open Locks`. Capitalisation and naming both move.

**All printed. Never harmonise**, either between classes or between a
description and its own table.

---

## Standing rule: no normalisation

The book's own inconsistencies are evidence and several of the findings
above depend on them. Reproduce every character as printed:

- **Dashes.** En-dash vs hyphen is not noise — the p.107 table is the
  only place in the book using en-dashes in d% ranges, and that is how
  it was identified. Never normalise.
- **Backslashes.** E1, E2 and E3 are literal backslashes on the page.
- **Spelling.** British throughout. Never Americanise.
- **Quotation marks, apostrophes, ellipses.** As printed.
- **Capitalisation.** Including oddities like `TREASURE:` in full caps
  on p.260 where the surrounding labels are title case.

If a transcription looks tidier than the book, something has been lost.


---

## Addendum — 2026-09-07, the repair pass

**E390 to E393 were assigned after the maintenance pass, by the repair pass
that closed out the project.** Each exists because a repair made it possible
or a fresh check found it; none was known when E61–E389 were assigned.

- **E390** could not be assigned earlier and the reason is the useful part:
  the site was a genuine printed double space that the delivered file had
  **normalised away**, so marking it `printed as-is` would have attached that
  claim to text which was not as printed. The maintenance pass recorded it as
  a deliberate omission. The repair pass restored the space and the ID
  followed. **Fix the transcription first, then log it — not the other way
  round.**
- **E391** is the third instance of E60's class and was found by rebuilding
  the master index against the audited rosters rather than against the book's
  own front-matter list. **Two of the three were found only because something
  else was being counted.**
- **E392** is the sixth wrong page number in file 32's Index of Tables and,
  like E381 and E382, does not carry the +12 compositor signature. It was
  found by a verifier checking a different claim — **the second of the six
  found that way — so the set is not demonstrably closed at six.**
- **E393** was found by the file 07 stat-line normalisation, which had to
  census every label in the file to run at all. **A mechanical pass that
  censuses its whole class finds defects the class was not being searched
  for.**

**Two retractions now stand, E16 and E365, and they fail in opposite
directions.** E16 described a gap that was not there, because it read one
page of a two-page table. E365 described a cell accurately and drew the wrong
conclusion from it, because the leave-alone list had already ruled on the
identical cell one table earlier and named only its own page. **The first was
a reading error; the second was a scoping error in the register itself.**
Three of the project's hardest items — `L Shield`, E16 and E365 — were
ambiguities in the project's own records rather than questions about OSRIC.
**When an item has been open for several passes and each new measurement
agrees with the last, suspect the record before suspecting the evidence.**
