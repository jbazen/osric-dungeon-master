# OSRIC SRD

The OSRIC rulebook, converted from PDF to Markdown, for use as a rules-lookup reference by Claude
(see the table in `../CLAUDE.md`).

- `markdown/` — one file per rulebook section (front matter through the master index)
- `osric.md` — all sections concatenated into a single file, in book order, for convenience. Check
  its own header for its current audit-status caveat before treating it as authoritative — prefer
  the individual section files in `markdown/` when accuracy matters.
- `errata.md` — log of the book's own printed errors (typos, misprinted tables, etc.) found during
  conversion. Inline comments like `<!-- printed as-is: see errata E51 -->` throughout `markdown/`
  and `osric.md` point here — they just confirm a given oddity is really printed that way in the
  book, not a transcription mistake. Not needed for day-to-day play; it's a reference for resolving
  those comments if one is ever worth double-checking.

Scanned page images/figures from the book are intentionally **not** included here — the OGL covers
the rules text, not the book's artwork/scans, so those are left out of this public repo pending a
separate decision on rights.

## Status

44 sections are in `markdown/` (see the reference table in `CLAUDE.md`), plus the merged `osric.md`
and the `errata.md` log. A full audit pass across all sections completed 2026-09-07 (see `osric.md`'s
own header for detail); further correction passes may still update individual files.

## License

OSRIC is released under the Open Gaming License v1.0a. The full license text is at
`markdown/33 licence.md` — that file governs use/redistribution of this directory's content.
