# Campaign Generation

Reference: `osric-srd/markdown/15 dungeons and generation.md` for dungeon stocking,
`osric-srd/markdown/16a urban and wilderness encounters.md` and `16b wilderness encounter tables.md`
for wilderness/urban content, and `../modules/README.md` + `running-modules.md` for published-module
campaigns.

## Two Ways to Start a Campaign

1. **Module-based**: Pick a converted module from `modules/`. Use its map and keyed encounters as
   the primary content — see `running-modules.md`.
2. **Generated**: Build a dungeon or wilderness area using the tables in
   `osric-srd/markdown/15 dungeons and generation.md` (room/corridor generation, stocking with
   monsters/treasure/traps/empty per the standard percentages) for sessions between or outside modules.

## Campaign State File

Create `campaigns/[campaign-name]/state.md` at campaign start and keep it current:

```markdown
# Campaign: [Name]

## Party
- [Character] — level, class, notable status (injured, cursed, etc.)

## Current Location
[Module name + room/area, or generated location]

## Game-Date & Time Tracking
- In-game date/time
- Last wandering-monster check: [turn/round]
- Rest/light source status (torches remaining, spells memorized today, etc.)

## Active Threads
- [Unresolved hooks, pursuing enemies, standing offers, faction reactions]

## Session Log
- [Session #] — [date] — [brief summary of what happened]
```

## Wilderness & Town Play

Between dungeon delves, use `14a exploration town planes.md` for town services (temples, shops,
sages, training) and the wilderness encounter tables for overland travel. Track travel time and
random encounter checks the same way you would underground turns.

## Pacing Across Sessions

- Open each session with a recap drawn from `state.md`, not from memory of the conversation.
- Close each session by updating `state.md` and all changed character sheets before ending.
- If a module is in progress, note exactly which keyed area/room the party is at or near, so the
  next session can resume precisely.
