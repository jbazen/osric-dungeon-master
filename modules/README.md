# Adventure Modules

Published AD&D adventure modules, converted to Markdown for use as campaign content. Each module
gets its own directory:

```
modules/
  [module-code]-[module-name]/
    markdown/            # Converted module text, one file per section/keyed area — mirrors the
                          # osric-srd/markdown/ convention rather than one flat file, since a full
                          # module can run just as long as a rulebook section set
    maps/                 # Map images/descriptions, if available
    handouts/             # Player handouts, if available
    README.md             # Module credits, original publisher, edition/printing notes
```

Example: `modules/b2-keep-on-the-borderlands/markdown/`

Some modules are large enough to warrant their own standalone repo instead of living here (e.g. when
the module is being transcribed independently, or kept in a separate private repo for licensing
reasons) — in that case this folder can hold just a pointer `README.md` noting where the real content
lives.

## Status

No modules have been added yet.

## Running a Module

See `../dm-instructions/running-modules.md` for how Claude should use these files during play —
including handling read-aloud text, keeping DM-only information hidden from players, and adapting
original AD&D 1e stat blocks to OSRIC where needed (usually a direct match).

## Licensing Note

Published modules are commercial products. Only add content you have the legal right to use (e.g.
modules you own, or those released under an open license). Document the specific license/rights for
each module in its own `README.md`.
