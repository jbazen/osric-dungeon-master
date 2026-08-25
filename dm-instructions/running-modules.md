# Running Published Modules

How to use converted content from `modules/[module-name]/module.md` during play. See
`../modules/README.md` for the expected file layout.

## Before the Session

1. Read the module's background/overview and note any DM-only secrets, plot hooks, or faction
   relationships that shouldn't be revealed to players directly.
2. Confirm which keyed area/room the party is at or approaching, per `campaigns/[name]/state.md`.
3. Note any wandering monster table specific to the module (many modules override or supplement the
   general OSRIC tables for their setting).

## During the Session

- **Read-aloud/box text**: Deliver the module's descriptive text to players close to as written when
  they first enter an area — this is meant to be read (or closely paraphrased), not summarized away.
- **Keyed encounters**: Use the module's stat blocks and encounter notes for that area. If a stat
  block uses original AD&D 1e terms that map directly to OSRIC (THAC0, AC, saves), use it as-is —
  OSRIC was designed for drop-in compatibility with 1e material.
- **DM-only information**: Secret doors, traps, monster tactics, and treasure contents come from the
  module's key — do not reveal them to players until discovered in-fiction (search, trigger, etc.).
- **Player choice over module structure**: Modules assume linear exploration but players may go off
  the module's expected path — improvise using the general dungeon/wilderness generation rules
  (`campaign-generation.md`) when they leave keyed content, and return to the module once they re-enter it.

## After the Session

Update `campaigns/[name]/state.md` with:
- Exact room/area reached or completed
- Monsters killed/fled, traps triggered/disarmed, treasure taken
- Any module-specific flags (doors unlocked, NPCs allied/killed, faction status changed)

## Adapting Non-OSRIC Stat Blocks

If a module was written for a different edition/retro-clone and its stat blocks don't map cleanly,
convert conservatively: match hit dice and rough AC/attack difficulty to the nearest OSRIC monster
entry rather than inventing new mechanics, and note the conversion in the module's own `README.md`
for consistency in future sessions.
