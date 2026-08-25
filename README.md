# OSRIC Dungeon Master

A 1st Edition AD&D-compatible Dungeon Master system powered by Claude, using the **OSRIC** (Old School
Reference and Index Compilation) rules to run classic dungeon-crawl campaigns — including published
AD&D adventure modules.

## What This Is

This repository contains instructions and reference materials that turn Claude into a capable OSRIC
Dungeon Master. It includes:

- **CLAUDE.md** — Core DM persona, tone guidelines, and session commands
- **dm-instructions/** — Detailed guidance for combat, character creation, NPCs, items, campaigns,
  spellcasting, and running published modules
- **osric-srd/** — The OSRIC rules reference, converted from the official OSRIC PDF to Markdown for
  lookup (populated separately — see below)
- **modules/** — Published AD&D adventure modules, converted for use as campaign content

## Status

The OSRIC rulebook conversion from PDF to Markdown is in progress — 37 sections are in
`osric-srd/markdown/` so far (ability scores, classes, spells, monsters, treasure, magic items, etc.
— see the reference table in `CLAUDE.md`), with more to come. Adventure modules will be added under
`modules/` as they're converted.

## Usage

1. Clone this repository
2. Open it with [Claude Code](https://claude.ai/claude-code) or add it as context in your Claude conversation
3. Start a new campaign or load an existing one

### Basic Commands

- `Start new campaign [name]` — Begin a new adventure, optionally based on a module in `modules/`
- `Load campaign [name]` — Resume an existing campaign
- `Create character` — Walk through OSRIC character creation
- `Save campaign` / `End session` — Save progress

Your campaign data is stored in a local `campaigns/` folder (excluded from git — it's your personal
play data, not shared content).

## Credits

### OSRIC

OSRIC (Old School Reference and Index Compilation) is a retro-clone of the 1st Edition Advanced
Dungeons & Dragons rules, released under the Open Gaming License v1.0a.

- **Original Content**: TSR, Inc. / Wizards of the Coast, based on the work of E. Gary Gygax
- **OSRIC Authors**: Stuart Marshall and Matthew Finch
- Full license text will be included at `osric-srd/markdown/33 licence.md` once the SRD conversion
  is added.

### Adventure Modules

Individual module credits are listed in each module's own directory under `modules/`.

## License

- DM instructions and CLAUDE.md: MIT License
- OSRIC SRD content: Open Gaming License v1.0a (see `osric-srd/markdown/33 licence.md` once added)
- Adventure module content: per original publisher/module license (documented per-module)
