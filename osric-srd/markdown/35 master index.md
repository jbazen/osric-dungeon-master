# OSRIC — Master Index

*OSRIC — master index routing every spell, monster and magic-item name to the transcription file that carries its full entry, and to the book page that entry begins on. Rebuilt 2026-09-07 from the corrected corpus, after the audit backlog closed.*

**Built from audited rosters, on the corrected files, and re-derived from the PDF.** The audit backlog closed on 2026-09-06: every file in `03 file manifest.md` has now had an independent audit run against it, audit batch 9 closing the last six. This index supersedes the batch 18 index, which carried a `⚠ Provisional` banner because it was built against a set in which 22 of 33 files were still unaudited. Every row below was produced mechanically, not typed: a per-file extractor read each source file's entry headings in document order and took each entry's book page from the file's own `<!-- p.N -->` markers — except the nine Golem and Lycanthrope rows, which take the section-heading page instead, for the reason each of those rows' Notes gives — and the result was then reconciled three ways — against `01 lists.md` (the book's own front-matter List of Spells / List of Monsters / List of Magic Items, itself audited PASS with no defects), against each source file's own header-line entry count, and against an **independent roster built from the PDF itself** by censusing the embedded display font in two-column reading order: `MyriadPro-BoldSemiCn` 9.5 pt entry headings across Chapters II and V (697 entries, including *Dread Wraith*'s embedded heading on book p.372), `MyriadPro-SemiboldSemiCn` 7.3–7.5 pt run-in entry labels across Chapter VI (345), and the same run-in face for the nine Golem and Lycanthrope entries in file 19, which the book sets as run-in labels under a shared stat table rather than as headings (9). **697 + 345 + 9 = all 1,051 entries**, and the diff returned **zero name mismatches in either direction and 1,042 of 1,051 pages matching**. The nine that do not match are the Golem and Lycanthrope rows, and they do not match by design: the PDF finds their run-in labels on pp.238 and 239, this index cites the section-heading pages 237 and 238, and each of those rows' Notes says so. Independently, every entry name was also searched for in the PDF text layer of the page the *marker* derivation gives it: 1,051 of 1,051 found. Forty-five pages were additionally rasterised and read by eye; they are listed under *What was and was not verified* below.

**What this index still does not guarantee.** It guarantees the *routing*: that the named entry exists in the named file and begins on the named book page. It does not guarantee the *contents* of those entries — the audits do that, and their findings, including the ones deliberately left unrepaired, live in `05 errata.md` and in the per-file records, not here. It does not re-litigate any errata item or leave-alone ruling; where a row's Note cites one, it cites it, it does not narrow it. Of the **249** distinct book pages that carry an indexed entry, **43** were rasterised and read for this rebuild and **206 were not**; and no entry's *text* was compared against the page for this pass. Where a page attribution rests on the PDF's embedded font and geometry layer rather than on a page image, the row is no better than that layer — which, on the evidence of this pass, is very good indeed, but it is not a page a human read. **All six of the page-marker placement defects this file records below as unrepaired were REPAIRED and independently verified later on 2026-09-07** — files 10, 11, 12 and 14a. That section is kept as written, because its finding stands: none of the six ever touched an indexed entry's page attribution, which was tested rather than assumed, and no row in this index changed as a result of the repair.

**Routing table — the one exception to this project's no-contents-block rule.** Every verbatim transcription file carries no contents block, no table of contents, and no anchor links, per `01 transcription template.md`'s standing convention — the consumer is a Claude instance that fetches one whole file and reads all of it, and a contents block would be duplicated content that costs tokens on every fetch and buys nothing. This file is different: its entire job is routing — *which file do I fetch for "Owlbear"?* — so it is allowed to be exactly the lookup table every other file is forbidden from being. State this here so nobody mistakes this file's structure for a violation of that rule.

## How to use this file

Look up a name in the tables below. The **File** column gives a short code; resolve it against the legend immediately below to the actual filename. The **Page** column is the book's own page number for where the entry begins in that file, and it follows the book's own front-matter list throughout, with **one exception**: *Ring of Spell Turning*, whose list cite is a printed error (E17) and whose row carries the real page with a Note. Separately — and this is not an exception to the list, which agrees — the nine **Golem** and **Lycanthrope** rows cite the page their section heading and shared stat table begin on, while each entry's own descriptive run-in falls on the *following* page; both pages are given in every one of those rows' Notes. A non-empty **Note** flags something about that specific row worth reading before you trust it — a printed-error correction, a book-level omission, an unusual routing, or a cross-reference.

**Entry names follow the book's own front-matter lists**, including their abbreviations (`Pro. from Evil*`, `Det. Minerals and Metals`), their reversibility asterisks, and their parenthetical alternate names. Three entries have no front-matter list row to take a name from — *Headband of Intellect*, *Portable Hole* and *Ring of Telekinesis* — and are named from the body entry instead, with the class-restriction abbreviation dropped for consistency with their neighbours.

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

- **00 front matter, 01 lists, 33 licence** — front matter, the source roster itself, and legal text. No spell/monster/magic-item entries of their own to index; `01 lists.md` is one of this index's own reconciliation sources, not something it indexes.
- **02, 03a, 03b, 04** (Chapter I, Creating a Character) — ability scores, races, classes, alignment, money, equipment. Player-facing character-creation material, not spell/monster/magic-item entries.
- **05 spells overview** — the spells chapter's introductory rules and mechanics sections. The spell *entries* themselves are in 06a through 11, which are indexed below; 05's own sections are not.
- **12, 13, 14a, 14b, 15, 16a, 16b** (Chapters III–IV, How to Play / Dungeons, Towns and Wildernesses) — rules text, hireling and henchman rules, the worked example dungeon and sample play session, dungeon generation tables, and encounter tables. None of these carry named spell/monster/magic-item entries in the indexed sense (the encounter *tables* in 16a/16b reference monster names that already have their own full entries in the Chapter V files, indexed below under Monsters).
- **30** (compiled tables, Appendix A) — 38 table and section headings (class Saving Throw/To Hit pairs, Thief Skills tables, the Melee/Missile Weapon tables, the Monster Equivalent Level table, and so on), not named creatures or magic items. It does not fit the name-indexed structure and is not forced into it here.
- **31** (afterword) — eleven paragraphs of prose, no discrete entries.
- **32** (index) — the book's own printed general index of terms plus its nested Index of Tables, keyed to the book's page numbers, not a list of spell/monster/magic-item names. It was used as a cross-check while building this file, **with cautions recorded rather than propagated**. Five of its Index-of-Tables page cites are known to be wrong in the book: the three `Treasure > Weapons` rows carrying a **+12 signature** (the compositor appears to have used PDF page numbers where printed folios belong) are **E387, E388 and E389**, and `Character Class > Ranger > Saving Throw` and `> To Hit`, both citing p.370 for a table on p.385, are **E381 and E382**. (E385 and E386 are a different class — a hyphen for an en dash, and a space after a slash — and are not page-number defects.) **A sixth wrong cite is recorded here for the first time, flagged and not resolved:** book p.396 (PDF 408) prints `Ring of Telekinesis – Maximum Weight   363`, but that table is printed on book **p.364**, inside the *Ring of Telekinesis* entry; its two neighbours, `Ring of Spell Turning – Result 363` and `Ring of Wizardry – Level(s) Doubled 364`, are both correct, so this one is off by one on its own and shows neither the +12 signature nor any systematic shift. Confirmed on a 600 dpi crop of PDF 408 and a 400 dpi crop of PDF 376 for this pass, after an independent verifier found it at 900–1200 dpi. **This is awkward for two claims made elsewhere in this file and the awkwardness is stated rather than smoothed over:** it means "five wrong cites" was the wrong number, and the *Ring of Telekinesis* row's own Note quotes this very back-index record as corroboration that the entry exists while silently disagreeing with the page it gives. The quotation is verbatim-correct and the row's page (364) is derived from the body and the PDF, not from file 32. **None of the six wrong numbers entered this index**, and file 32 was never used as a page-number source for any row; only its *presence or absence* of a term was consulted. **Both of those were closed later the same day: the sixth cite is now `E392`, and file 32 carries a marker on that record.** On 2026-09-07 file 32 also had 300 unprinted bold Index-of-Tables nodes stripped; that pass changed no body text and nothing this index cites.
- **34 figures** — the register of images, vector lettering and other non-text page furniture excluded from the transcriptions. No entries.
- **05 errata** — the errata register itself. This index cites it; it does not index it.

## Count reconciliation

This index carries **1,051 entry rows** — **414 spells, 292 monsters, 345 magic items** — plus **1 cross-reference row** (`L Shield +1, Missile Deflector`), for 1,052 table rows in total. Every one of the 1,051 was re-derived for this rebuild; none was carried over on trust.

Against the book's own front-matter lists in `01 lists.md`, which total an audited **1,048** (414 spells, 292 monsters, 342 magic items):

- **Spells: 414 = 414, exact.** Cleric 76 (06a 38 + 06b 38), Druid 78, Magic User 194 (08 65 + 09 64 + 10 65), Illusionist 66. Every one of the 414 maps to exactly one row, in the book's own order, on the same page the front-matter list cites.
- **Monsters: 292 = 292, exact.** 291 of them in the Chapter V files (17a 10 + 17b 24 + 18 26 + 19 33 + 20 30 + 21 43 + 22a 22 + 22b 20 + 23a 23 + 23b 19 + 24 41), plus *Dread Wraith*, whose only appearance in the book is the stat block embedded in the *Deck of Many Things* entry in file 29b. File 17a's own header line says "17 entries/sections": that is 10 indexed entries plus 7 section and sub-section headings (MONSTER STATISTICS, TRIBAL SPELL CASTERS, SHAMAN, WITCH DOCTOR, OPTIONAL RULES FOR TRIBAL SPELL CASTERS, MEN, DEMI-HUMANS), which are not entries and are not indexed. File 19's 33 comprises 1 (Uduk, continued from file 18) + 15 devils + 8 dinosaur groups + 4 golems + 5 lycanthropes; its golems and lycanthropes are the only Chapter V entries the book sets as **run-in bold labels under a shared stat table** rather than as display headings, which is why a heading-only extractor undercounts that file by nine.
- **Magic items: 345 against the list's 342 — a gap of three, all of them the same defect on the book's side.** All three are genuinely printed and fully described in the body, and all three are missing from the book's own front-matter List of Magic Items on book p.viii. Two are **E60**: *Headband of Intellect* (book p.353) and *Portable Hole* (book p.358). **The third is new and is flagged, not resolved: *Ring of Telekinesis* (book p.364).** In every case `01 lists.md` transcribes its page correctly, omission included, and **none of the three may ever be added to it.** Each is indexed here from the file that carries its body entry, with a Note.

Against the batch 18 index's **1,050 / 414 / 292 / 344**: the difference is exactly one row, *Ring of Telekinesis*, which that index did not carry because it was built from the front-matter list that omits it. See *What changed since the batch 18 index*.

Against the manifest: `03 file manifest.md`'s front-matter row records "List of Spells (414), List of Monsters (292), List of Magic Items (342) — 1,048 entries", which is the list's own count and agrees. **One manifest sentence is now wrong by one and was not changed here:** the file-29a row states its 33 entries are an "exact match against the audited roster in `01 lists.md`". The front-matter list carries 32 for that range (15 rings + 17 cursed items); the file's 33 is right and the list is short by *Ring of Telekinesis*. Flagged for a coordinator, not corrected by this pass.

## Cross-references and synonyms — the convention used here, stated explicitly

The book gives several entries an alternate name in parentheses directly in its own front-matter list — "Bandit (Brigand)," "Buccaneer (Pirate)," "Dervish (Nomad)," "Caveman (Tribesman)," and others. These print as **one entry**, not two cross-referenced headings, so this index gives each a single row under its primary printed name, parenthetical included exactly as printed, rather than adding a second "see" row under the alternate name. Nothing in this book's own three front-matter lists takes the form of a bare cross-reference (a hypothetical "Faerie Creatures — see Sylvan"); none were found while building this index. If one turns up in a future pass, the convention for it is: **a second row pointing at the primary entry's own File/Page, with the Note column marked as a cross-reference — not folded silently into the primary row's page cite.**

**One cross-reference row exists, and only one.** `L Shield +1, Missile Deflector` sits immediately above `Large Shield +1, Missile Deflector`, pointing at the same File and Page. This is not a naming choice by this index: the book prints the name both ways, `L Shield` in the front-matter list on book p.vii and `Large Shield` in the body entry on book p.339. That is **E58**, and both files are correct — do not harmonise them. The entry is routed under the body reading, which is the entry itself, and the front-matter spelling gets its own row so that either lookup finds it.

**One spelling pair is handled by Note rather than by a second row.** The front-matter List of Monsters prints `Werewold` where file 19's body prints `Werewolf` — **E11**, a single printed misspelling of one word rather than a genuine dual printing. The row sorts under the list's `Werewold`; the Note gives the body spelling so a search for either lands on it.

**One monster is a genuine structural exception, not a naming one:** *Dread Wraith* prints in the book's own List of Monsters out of sequence, after Yeti, pointing at page 372 — a confirmed leave-alone-list oddity, not something to correct — but its only appearance anywhere in the book's body text is as a stat block embedded inside the *Deck of Many Things* magic-item entry in file 29b. It has no entry of its own anywhere in the Monsters chapters. It is indexed below under Monsters, filed at 29b, flagged accordingly, precisely so a reader searching Monsters for Dread Wraith is routed correctly rather than left to conclude it was missed.

## Unrepaired page-marker defects — tested, not assumed

Six page-marker placement defects were found on 2026-09-07 and deliberately **not** repaired: file `10` at p.105 and p.108; file `11` at p.112; file `12` at p.126 and p.133; file `14a` at p.149. Files 12 and 14a are not indexed here. **Files 10 and 11 are.** Their effect on this index was tested against the PDF rather than taken on trust, and the finding is:

- **File 10, `<!-- p.105 -->`.** The marker sits after the whole *Spider Climb* stat block instead of before its last two lines. Book p.105 (PDF 117, rasterised and read) opens mid-*Spider Climb*, with `Casting Time: 1 segment` and `Saving Throw: None` at the head of column 1; the *Spider Climb* heading and the rest of its stat block are on p.104. Two stat lines are therefore misattributed in the file. **The entry's own page is unaffected: *Spider Climb* is indexed at p.104**, which is what `01 lists.md`, the PDF font roster and the raster all give.
- **File 10, `<!-- p.108 -->`.** The same shape at *Time Stop*, but larger: **four** stat lines are misattributed here, not two. Book p.108 (PDF 120, rasterised and read) opens mid-*Time Stop* stat block with `Area of Effect`, `Components`, `Casting Time` and `Saving Throw` at the head of column 1; the heading is on p.107. **Indexed at p.107**, agreeing with the list, the font roster and the raster.
- **File 11, `<!-- p.112 -->`.** The marker sits below the `## ILLUSIONIST SPELLS` chapter heading instead of above it, so the heading itself carries no page. Book p.112 (PDF 124, rasterised and read) opens with that heading, and the file's first indexed entry, *Alter Reality*, follows it on the same page. **No indexed entry is affected**; every illusionist entry's page is unchanged.

**Conclusion: none of the six unrepaired defects changes the File or Page of any indexed entry.** The report that found them predicted this for files 10 and 11 on the grounds that the misplaced markers sit below stat lines and a chapter heading rather than below entry headings; that prediction was checked here against three rasterised pages and holds. The defects remain in the corpus, unrepaired, exactly as ruled.

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
| Flesh | 237 | 19 | the entry begins on p.237 with the GOLEMS section heading and the four-column stat table (Clay / Flesh / Iron / Stone); its own descriptive paragraph, the run-in `**Flesh Golem:**`, begins on **p.238**. Both pages verified on the raster (PDF 249, 250). `01 lists.md` and this index cite 237, the page the entry itself starts on; the file's nearest preceding page marker for the descriptive paragraph is 238 — one of two such places, the other being the Lycanthropes block below. |
| Stone | 237 | 19 | the entry begins on p.237 with the GOLEMS section heading and the four-column stat table (Clay / Flesh / Iron / Stone); its own descriptive paragraph, the run-in `**Stone Golem:**`, begins on **p.238**. Both pages verified on the raster (PDF 249, 250). `01 lists.md` and this index cite 237, the page the entry itself starts on; the file's nearest preceding page marker for the descriptive paragraph is 238 — one of two such places, the other being the Lycanthropes block below. |
| Iron | 237 | 19 | the entry begins on p.237 with the GOLEMS section heading and the four-column stat table (Clay / Flesh / Iron / Stone); its own descriptive paragraph, the run-in `**Iron Golem:**`, begins on **p.238**. Both pages verified on the raster (PDF 249, 250). `01 lists.md` and this index cite 237, the page the entry itself starts on; the file's nearest preceding page marker for the descriptive paragraph is 238 — one of two such places, the other being the Lycanthropes block below. |
| Clay | 237 | 19 | the entry begins on p.237 with the GOLEMS section heading and the four-column stat table (Clay / Flesh / Iron / Stone); its own descriptive paragraph, the run-in `**Clay Golem:**`, begins on **p.238**. Both pages verified on the raster (PDF 249, 250). `01 lists.md` and this index cite 237, the page the entry itself starts on; the file's nearest preceding page marker for the descriptive paragraph is 238 — one of two such places, the other being the Lycanthropes block below. |

### Lycanthropes

| Entry | Page | File | Note |
|---|---|---|---|
| Werebear | 238 | 19 | the entry begins on p.238 with the LYCANTHROPES section heading and the five-column stat table, which straddles the p.238/239 break; its own descriptive paragraph, the run-in `**Werebear:**`, is on **p.239**. Both pages verified on the raster (PDF 250, 251). Cited here as 238, the page the entry itself starts on. |
| Wereboar | 238 | 19 | the entry begins on p.238 with the LYCANTHROPES section heading and the five-column stat table, which straddles the p.238/239 break; its own descriptive paragraph, the run-in `**Wereboar:**`, is on **p.239**. Both pages verified on the raster (PDF 250, 251). Cited here as 238, the page the entry itself starts on. |
| Wererat | 238 | 19 | the entry begins on p.238 with the LYCANTHROPES section heading and the five-column stat table, which straddles the p.238/239 break; its own descriptive paragraph, the run-in `**Wererat:**`, is on **p.239**. Both pages verified on the raster (PDF 250, 251). Cited here as 238, the page the entry itself starts on. |
| Weretiger | 238 | 19 | the entry begins on p.238 with the LYCANTHROPES section heading and the five-column stat table, which straddles the p.238/239 break; its own descriptive paragraph, the run-in `**Weretiger:**`, is on **p.239**. Both pages verified on the raster (PDF 250, 251). Cited here as 238, the page the entry itself starts on. |
| Werewold | 238 | 19 | the entry begins on p.238 with the LYCANTHROPES section heading and the five-column stat table, which straddles the p.238/239 break; its own descriptive paragraph, the run-in `**Werewolf:**`, is on **p.239**. Both pages verified on the raster (PDF 250, 251). Cited here as 238, the page the entry itself starts on. **Spelling:** the front-matter List of Monsters prints `Werewold` (the name used for this row, and the reason it sorts here); the body entry in file 19 prints `Werewolf`. That misprint is **E11** — reproduced on both sides, not harmonised. Search either spelling; this is the same entry. |

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
| Dread Wraith | 372 | 29b | embedded in the *Deck of Many Things* entry, not a standalone heading; printed out of sequence in the book's own List of Monsters (after Yeti), pointing into the Artifacts page range — reproduced as printed, see the leave-alone list in `05 errata.md`. Its stat block is the only appearance of this monster anywhere in the book; there is no entry for it in Chapter V. Page re-verified on the raster (PDF 384). |

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
| L Shield +1, Missile Deflector | 339 | 26 | **cross-reference row — see `Large Shield +1, Missile Deflector` immediately below, same File and Page.** This is the spelling the book's own front-matter List of Magic Items (book p.vii) prints; the body entry (book p.339) prints `Large Shield`. **E58** — the book contradicts itself and both files reproduce their own page correctly. Do not harmonise them; both spellings are indexed so either lookup routes. |
| Large Shield +1, Missile Deflector | 339 | 26 | **See errata E58.** Not a transcription conflict: the book prints it both ways. The front-matter List of Magic Items (book p.vii) prints `L Shield`, and file 01 correctly transcribes that; the body entry (book p.339) prints `Large Shield`, and file 26 correctly transcribes that. Both confirmed at 600 dpi and by word box; the body reading re-confirmed on the raster of PDF 351 for this rebuild. Indexed here under the body reading, which is the entry itself; the front-matter spelling has its own cross-reference row above. |

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
| Headband of Intellect | 353 | 28 | **E60.** Not in the book's own front-matter List of Magic Items (book p.viii, PDF 10) — genuinely printed and fully described in file 28's body on book p.353, between *Hat of Disguise* and *Helm of Brilliance*. Both facts re-verified on the raster for this rebuild (PDF 365 for the body entry, PDF 10 for the omission). **`01 lists.md` is not at fault** — it transcribes its page exactly as printed, omission included, and this entry must never be added to it. Routed from file 28. |
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
| Portable Hole | 358 | 28 | **E60.** Not in the book's own front-matter List of Magic Items (book p.viii, PDF 10) — genuinely printed and fully described in file 28's body on book p.358, between *Plentiful Vessel* and *Restorative Ointment*. Both facts re-verified on the raster for this rebuild (PDF 370 for the body entry, PDF 10 for the omission). **`01 lists.md` is not at fault** — it transcribes its page exactly as printed, omission included, and this entry must never be added to it. Routed from file 28. |
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
| Ring of Spell Turning | 363 | 29a | the book's own front-matter List of Magic Items prints page **63** for this entry where its neighbours print 363 and 364 — **E17**, verified at 600 dpi: the glyphs really are `63`, with no clipped leading digit, and re-read on the PDF 10 raster for this rebuild. That `363` was intended is an inference from the surrounding sequence, not something the page states. The **363** cited here is not taken from that list: it is derived from file 29a's own page markers and independently confirmed against the PDF, where the entry sits on book p.363 between *Ring of Spell Storing* (363) and *Ring of Swimming* (364). |
| Ring of Swimming | 364 | 29a |  |
| Ring of Telekinesis | 364 | 29a | **Logged as E391 on 2026-09-07 — a third omission of the E60 class, not previously recorded anywhere in this project.** This entry is not in the book's own front-matter List of Magic Items (book p.viii, PDF 10), whose RINGS block runs Charisma → Wizardry in fifteen rows with no Telekinesis. It is genuinely printed and fully described in file 29a's body on book p.364, between *Ring of Swimming* and *Ring of Three Wishes*, and the book's **own back-of-book index** carries it (`32 index.md`: "Ring of Telekinesis – Maximum Weight 363"). Both the body entry and the front-matter omission were verified on the raster for this rebuild (PDF 376 and PDF 10). **`01 lists.md` is not at fault** and this entry must not be added to it. Both consequences are now closed: a **new erratum, E391**, was opened rather than extending E60, and `03 file manifest.md`'s file-29a sentence has been corrected. The back-index record it cites is itself wrong about the page and is logged as **E392**; this row's page, 364, is derived from the body and the PDF, not from file 32. |
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

---

## What was and was not verified — 2026-09-07

**Rasterised at 150 dpi and read by eye: 45 PDF pages — 44 in the arabic zone plus book p.viii (PDF 10).** Of the 44 arabic pages, **43 carry an indexed entry**; the forty-fourth, PDF 251 (book p.239), carries none, because the Lycanthrope rows are filed at 238. So the coverage arithmetic is **249 indexed pages = 43 rasterised + 206 not**. Book-page offset re-confirmed first, both by reading printed folios (PDF 13→1, 100→88, 213→201, 249→237, 251→239, 320→308, 376→364, 386→374, 400→388) and by the front-matter roman zone (PDF 10→viii): **arabic book p.N = PDF page N+12; roman i–x = PDF 3–12.**

| PDF page | Book page | What it was rasterised to check |
|---|---|---|
| 10 | viii | The front-matter List of Magic Items. Confirms the RINGS block runs fifteen rows, Charisma → Wizardry, with **no Ring of Telekinesis**; confirms `Hat of Disguise 353` → `Helm of Brilliance 353` with **no Headband of Intellect**; confirms `Plentiful Vessel 358` → `Restorative Ointment 358` with **no Portable Hole**; and confirms *Ring of Spell Turning* really does print `63` (E17). |
| 117, 120, 124 | 105, 108, 112 | The three unrepaired page-marker defects in indexed files 10 and 11. |
| 77, 85, 90, 95, 97, 100, 103, 105, 127 | 65, 73, 78, 83, 85, 88, 91, 93, 115 | Random sample, spell files 07–11: Predict Weather (65), Clairvoyance (73), Duo-Dimension (78), Flame Arrow (83), Grasping Hand (85), Infravision (88), Locate Object (91), Massmorph (93), Hallucinatory Terrain (115). |
| 213 | 201 | **Goblin** — corrected in audit batch 5 from p.200. |
| 218, 233, 267, 273, 316 | 206, 221, 255, 261, 304 | Random sample, monster files: Giant, Fire (206), Demonette (221), Boar, Warthog (255), Indricotherium (261), Remorhaz (304). |
| 249, 250, 251 | 237, 238, 239 | The Golems and Lycanthropes structure: stat tables on 237 and 238/239, descriptive run-ins on 238 and 239. |
| 258 | 246 | **Ghast** — the page whose marker audit batch 6 moved. |
| 289 | 277 | **Chimæra** and **Cockatrice** — corrected in audit batch 7 from p.278. |
| 313, 314, 315 | 301, 302, 303 | **Pegasus, Phoenix, Piercer, Pseudo-Dragon** — the four attributions audit batch 7 found wrong in file 23b. |
| 319, 320 | 307, 308 | **Rust Monster, Sahuagin, Scorpion, Sea Hag** — corrected in audit batch 8 from 306/307. |
| 351, 352 | 339, 340 | `Large Shield +1, Missile Deflector` printed in full (E58), and a random-sample check on Luck Blade (340). |
| 361, 364, 365 | 349, 352, 353 | Cube of Force (349) as a random sample, and the file-27 pages whose fifteen attributions audit batch 8 corrected: all four p.352 entries and all nine p.353 entries confirmed. |
| 365, 370 | 353, 358 | **Headband of Intellect** and **Portable Hole** in the body (E60). |
| 366, 369 | 354, 357 | Random sample, file 28: Horn of Goodness/Evil (354), Mirror of Opposition (357). |
| 374, 376, 378, 379, 380 | 362, 364, 366, 367, 368 | Random sample, file 29a, plus **Ring of Telekinesis** on p.364 and the 29a/29b shared p.368 seam. |
| 381, 382, 383 | 369, 370, 371 | The *Deck of Many Things* neighbourhood, after file 29b's `p.371` marker moved in audit batch 9. |

**Resolutions, stated so they are not confused.** Every raster this rebuild produced and read was **150 dpi**, plus a 600 dpi crop of PDF 408 and a 400 dpi crop of PDF 376 taken for the sixth file-32 cite recorded above. The **600 dpi** confirmations cited inside the *Ring of Spell Turning* (E17) and *Large Shield +1, Missile Deflector* (E58) Notes belong to the **earlier** rulings that established those errata, not to this pass; where those Notes say the point was "re-read" or "re-confirmed" for this rebuild, that re-reading was at 150 dpi. The substance of both survived an independent verifier's 900 dpi re-read, so this is looseness in the Notes' wording rather than an error in them, and it is recorded here rather than by rewriting the rows.

**Whole-corpus checks that were not samples.** An independent entry roster was built from the PDF's own embedded font and geometry layer, in two-column reading order, across book pp.36–374 — 697 display-font headings, 345 Chapter VI run-in labels, and the 9 file-19 Golem/Lycanthrope run-ins — and diffed against this index: **1,051 of 1,051 entries matched on name, and 1,042 of 1,051 matched on page.** The nine that differ are the Golem and Lycanthrope rows, and the difference is deliberate and documented rather than a defect: the PDF puts their run-in labels on pp.238 and 239, this index cites the section-heading pages 237 and 238 — the same pages the book's own front-matter list gives — and every one of those nine Notes states both. Separately, every entry name was searched for in the PDF text layer of the page its file's markers give it: 1,051 of 1,051 found. Neither check consulted `01 lists.md` or the batch 18 index.

**Not checked, stated plainly.** No entry's *body text* was compared against the page for this pass — that is the audits' job and it is done. **206 of the 249** distinct book pages carrying an indexed entry were never rasterised for this rebuild; rows on them rest on the font/geometry layer plus `01 lists.md` plus each file's own markers — all three agreeing — but on no page image read for this pass. No boundary between adjacent files was re-verified; the audits' boundary findings were taken as given. Nothing in files 12, 14a, 30 or 32 was examined beyond what is stated above. Of the six wrong page cites now known in file 32's Index of Tables, the five carrying errata IDs (E381, E382, E387, E388, E389) were not re-measured — they were simply kept out; only the sixth, the *Ring of Telekinesis* record on book p.396, was measured on a raster by this pass, and no systematic re-check of the remaining Index-of-Tables cites was run, so a seventh may exist.

## What changed since the batch 18 index — 2026-09-07

**No File or Page cite changed. Not one, in 1,050 carried-over rows.** That is the single most important finding of this rebuild and it needs explaining, because the brief for this work expected otherwise. The batch 18 index took its **Page** column from `01 lists.md` — the book's own front-matter lists — not from the transcription files' page markers. The twenty-eight heading attributions the audits corrected, and file 29b's `p.371` marker move, were corrections that brought the *files* into agreement with those lists; they did not move any number the index was citing. This was tested, not assumed: the derived roster was compared row by row against the batch 18 index (0 File/Page differences outside the two rows below) and independently against the PDF's own font roster (0 differences of any kind). Specifically confirmed unchanged and correct: Goblin 201, Ghast 246, Chimæra 277, Cockatrice 277, Pegasus 301, Phoenix 302, Piercer 303, Pseudo-Dragon 303, Rust Monster 307, Sahuagin 307, Scorpion 308, Sea Hag 308, all fifteen of file 27's corrected entries, and *Deck of Many Things* 371 with its neighbours *Book of Infinite Spells* 370 and *Hammer of Thunderbolts* 373.

**Two rows added.**

| Row | Change |
|---|---|
| **Ring of Telekinesis** (Magic Items → Rings) | **ADDED — 29a, p.364.** Absent from the batch 18 index entirely, because that index was built from the front-matter list, which omits this entry. A third omission of the E60 class, not previously recorded anywhere in this project. See the row's own Note. |
| **L Shield +1, Missile Deflector** (Magic Items → Magic Armour And Shields) | **ADDED as a cross-reference row — 26, p.339**, pointing at `Large Shield +1, Missile Deflector` on the same File and Page. The batch 18 index carried only the body spelling. E58 having settled that the book genuinely prints it both ways, both spellings are now findable. This is a cross-reference row, not a 1,052nd entry; it is excluded from the entry counts above. |

**Fourteen rows had their Note changed. No other column moved on any of them.**

| Row | Old → New |
|---|---|
| Golems → **Flesh**, **Stone**, **Iron**, **Clay** (4 rows) | Note added where there was none. Page unchanged at 237, File unchanged at 19. The Note now records that the entry begins on p.237 with the section heading and stat table while its descriptive paragraph begins on p.238, and that this is one of two places where the marker-derived page and the cited page differ, the other being the Lycanthropes block. |
| Lycanthropes → **Werebear**, **Wereboar**, **Wererat**, **Weretiger** (4 rows) | Note added where there was none. Page unchanged at 238, File unchanged at 19. Same structural fact: stat table opens on p.238, descriptive paragraphs are on p.239. |
| Lycanthropes → **Werewold** | Note added where there was none. Page unchanged at 238, File unchanged at 19. Carries the structural note plus the `Werewold`/`Werewolf` spelling pair and its E11 cite, so a search for either spelling routes. |
| Monsters → Other Creatures → **Dread Wraith** | Note extended. Page unchanged at 372, File unchanged at 29b. Added: that its embedded stat block is the monster's only appearance in the book and there is no Chapter V entry for it, and that the page was re-verified on the raster. |
| Magic Armour And Shields → **Large Shield +1, Missile Deflector** | Note rewritten. Page unchanged at 339, File unchanged at 26. Now cites **E58** as a settled erratum rather than as a resolution dated in the note body, records that the body reading was re-confirmed on this rebuild's raster of PDF 351, and points at the new cross-reference row above it. |
| Miscellaneous Magic → **Headband of Intellect** | Note rewritten. Page unchanged at 353, File unchanged at 28. Now cites **E60** by ID (the batch 18 note predated the ID and pointed at the backlog document), names the neighbouring entries it sits between, and records that both the body entry and the front-matter omission were re-verified on the raster. |
| Miscellaneous Magic → **Portable Hole** | Note rewritten. Page unchanged at 358, File unchanged at 28. Same change as *Headband of Intellect*. |
| Rings → **Ring of Spell Turning** | Note rewritten. Page unchanged at 363, File unchanged at 29a. Now states explicitly what the batch 18 note left implicit: the `363` cited here is **not** taken from the front-matter list — it is derived from file 29a's own page markers and independently confirmed against the PDF — and that `363` was *intended* where the page prints `63` remains an inference (E17), not something the page states. The E17 ruling is cited, not narrowed. |

**Nothing was removed.** All 1,050 batch 18 rows survive, under the same names, in the same sections, in the same order.

**Prose sections changed:** the `⚠ Provisional` banner is gone, replaced by a statement of provenance and an explicit statement of what this index still does not guarantee; *How to use this file* now explains the entry-naming convention, names the single front-matter page-cite exception (E17) and separates it from the nine Golem and Lycanthrope rows, which agree with the front-matter list and differ only from the marker derivation; *What is not indexed here* gains rows for `34 figures.md` and `05 errata.md` and a caution about file 32's wrong Index-of-Tables page cites — the five with errata IDs and a sixth recorded here for the first time; *Count reconciliation* is rewritten around re-derived counts; *Cross-references and synonyms* gains the E58 cross-reference row convention and the E11 Note convention; and two sections are new — *Unrepaired page-marker defects* and *What was and was not verified*.

**Flagged, not resolved, for a coordinator.** (1) *Ring of Telekinesis* is a third front-matter omission of the E60 class; whether E60 is extended or a new erratum opened is not this pass's call, and `05 errata.md` was not touched. (2) `03 file manifest.md`'s file-29a row says that file's 33 entries are an "exact match against the audited roster in `01 lists.md`"; the list carries 32 for that range. The manifest was not edited. (3) **A sixth wrong page cite in file 32's Index of Tables, not recorded anywhere in this project before now:** book p.396 (PDF 408) prints `Ring of Telekinesis – Maximum Weight   363` for a table printed on book **p.364**. Found by an independent verifier at 900–1200 dpi and confirmed here on a 600 dpi crop of PDF 408 against a 400 dpi crop of PDF 376; its two neighbouring records are both correct, so it is off by one on its own, with neither the +12 signature of E387–E389 nor the p.370 shape of E381–E382. **File 32 was not edited, no erratum was opened, and the *Ring of Telekinesis* row's page (364, derived from the body and the PDF, not from file 32) was not changed.** **CLOSED — it is now `E392`.** (4) No transcription file was edited by this pass. This index is the only file it wrote.

**ALL THREE OF THE ABOVE WERE CLOSED LATER ON 2026-09-07 by the repair pass that followed this rebuild:** *Ring of Telekinesis* is logged as **E391**, a third entry of the E60 class, with `01 lists.md` confirmed not at fault and instructed never to have it added; the sixth wrong Index-of-Tables cite is logged as **E392** and file 32 now carries its marker; and `03 file manifest.md`'s file-29a sentence has been corrected to read 32 + 1. **No row in this index changed** — the routing data was verified correct before any of it.
