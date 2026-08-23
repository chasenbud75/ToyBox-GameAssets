# Asset provenance

Every file in this repo, where it came from, and what its licence permits.

**Why this file exists.** This repo is **public**, and the game loads from it by
raw URL — so each file is downloadable on its own, not just as part of a build.
Several "free" music licences (Pixabay's included) allow use *inside* a product
but forbid distributing the file **on a standalone basis**, which is exactly what
a raw URL does. Anything listed here as unresolved is worth replacing with a
licence that permits redistribution — CC0 is the clean answer.

If a store, a platform or a collaborator ever asks where something came from,
this file is the answer. Fill a row in when you add a file, not later.

---

## Audio — ACTION NEEDED

Sourced from **Pixabay** unless noted. Pixabay's Content Licence permits
commercial use with no attribution, but **prohibits redistributing content on a
standalone basis** — the open question for a public asset repo.

| file | used by | source | title / artist | licence | added | resolved? |
|------|---------|--------|----------------|---------|-------|-----------|
| `dir_Parlour_music.mp3` | Director's Cut — Parlour | Pixabay | _TODO: track page URL_ | Pixabay Content Licence | _TODO_ | ⚠️ standalone hosting |
| `dir_Space_music.mp3` | Director's Cut — Deep Space | Pixabay | _TODO_ | Pixabay Content Licence | _TODO_ | ⚠️ |
| `dir_attic_Music.mp3` | Director's Cut — Attic | Pixabay | _TODO_ | Pixabay Content Licence | _TODO_ | ⚠️ |
| `dir_BumperChaos_Music.mp3` | Bumper Chaos | Pixabay | _TODO_ | Pixabay Content Licence | _TODO_ | ⚠️ |
| `race_crowd.mp3` | Bumper Chaos crowd | _TODO_ | _TODO_ | _TODO_ | _TODO_ | ⚠️ |

**To resolve a row:** paste the track's page URL and the artist name, then either
(a) confirm the licence permits redistribution, or (b) replace the track with a
CC0 one and update the row. CC0 sources that suit a game: OpenGameArt (filter
CC0), Kenney.nl, Freesound (filter CC0). Free-with-attribution is also fine —
the game has a credits screen — but the attribution then belongs in the game,
not only here.

Synthesised beds in `lib/boardSounds.js` are generated at runtime from
oscillators. They are code, not recordings, and raise no licensing question.

## Video

| file | used by | source | licence | notes |
|------|---------|--------|---------|-------|
| `race_clip_missile.mp4` | replay pop-up | AI-generated (Higgsfield) | per generator's terms | re-encoded locally; original watermark cropped |
| `race_clip_mud.mp4` | replay pop-up | AI-generated (Higgsfield) | per generator's terms | as above |
| `race_clip_tossed.mp4` | replay pop-up | AI-generated (Higgsfield) | per generator's terms | as above |
| `race_clip_zombie.mp4` | replay pop-up | AI-generated (Higgsfield) | per generator's terms | as above |
| `dir_detonate.mp4` | Director's Cut detonation | _TODO_ | _TODO_ | |

## Images — 169 files

Board art, item art, car art and the Director's Cut frame library. All either
**generated** (Gemini, and nano-banana-pro via Higgsfield) or **authored by the
owner in Photoshop**, then processed locally by the scripts in
`Base44/Toy Box Rumble/Assets/Game/BumperChaos/`.

No third-party stock imagery is knowingly present. Ownership of generated images
follows the terms of the service that produced them — worth reading once if this
ever ships commercially, since those terms differ by provider and change.

Notable derived files, so their provenance is not mistaken for stock:

| file | how it was made |
|------|-----------------|
| `race_board.jpg` | painted over the generated template for track 1 |
| `race_board2.jpg` | painted by the owner over `track2_template.png`, then cleaned and arrowed by script |
| `race_track3.jpg` | ditto for track 3, with the traffic light lifted onto its own overlay |
| `race_track2_bridge.png`, `race_track2_shadow.png` | bridge layer exported by the owner; shadow generated from its silhouette |
| `race_track3_takeoff/landing/pole/shadow.png` | layers exported by the owner, aligned to the traced geometry by script |

---

_Last reviewed: 2026-08-23._
