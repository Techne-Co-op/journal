# journal

`journal.techne.coop` — the cooperative's journal surface, served by GitHub Pages from `main`.

**Status: exploration. Nothing here is adopted, and nothing here changes the Common Information System's schema.**

## What is at the root

The Open World shell and the **Daybook public beta**, brought over from [`Techne-Co-op/open-world`](https://github.com/Techne-Co-op/open-world) on 2026-08-31 at the steward's direction. The Daybook is at [`/daybook/`](/daybook/).

The Daybook beta holds **no data of its own**: it is in-memory, its classifier is a word-pattern stand-in for the live reader, and its seed is a labelled demonstration. Members' real first names appear in that seed against invented entries; the label on every view says so.

Its governing documents, and the decisions D-01 through D-05 that shaped it, live in the `open-world` repository rather than here.

## What is at `/v1/`

The first journal, preserved whole and still reachable at [`/v1/`](/v1/): the architecture note, the design system and its bloom variant, the encyclopedia, common-work, work and capture, and the original seven-page Daybook. Forty-eight commits of work.

It was moved rather than deleted. Its internal links were rewritten to follow the move and nothing in it was otherwise edited. **Its Supabase wiring points at the `Techne Daybook` project, which is currently paused**, so its live surfaces do not presently reach a backend.

## The record, and the halt

The app caches its shell and never the record: the halt wins over offline. Identity is read from the Common Information System through the same anon client and the same `agents` / `memberships` / `role_grants` reads the intranet uses; authorization is row-level security on the server, never a decision this page makes.
