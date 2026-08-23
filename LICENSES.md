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

## Audio — all CC0

Replaced 2026-08-23. Every track is **CC0** (public domain dedication): no
attribution required, and redistribution permitted — which is what matters here,
since this repo is public and the game loads each file by raw URL rather than
only inside a build. The tracks that were here before came from Pixabay, whose
licence forbids standalone redistribution.

| file | used by | title | author | source | licence |
|------|---------|-------|--------|--------|---------|
| `dir_attic_Music.mp3` | Director's Cut — Attic | Horror Loop | TinyWorlds | [opengameart.org/content/horror-loop](https://opengameart.org/content/horror-loop) | CC0 |
| `dir_Parlour_music.mp3` | Director's Cut — Parlour | Night Prowler | Section 31 | [opengameart.org/content/night-prowler](https://opengameart.org/content/night-prowler) | CC0 |
| `dir_Space_music.mp3` | Director's Cut — Deep Space | My Very Own Dead Ship | madeso | [opengameart.org/content/background-space-track](https://opengameart.org/content/background-space-track) | CC0 |
| `dir_BumperChaos_Music.mp3` | Bumper Chaos | Determined Pursuit | Emma_MA | [opengameart.org/content/determined-pursuit-epic-orchestra-loop](https://opengameart.org/content/determined-pursuit-epic-orchestra-loop) | CC0 |
| `race_crowd.mp3` | Bumper Chaos crowd | Applause after a concert | Amada44 | [commons.wikimedia.org](https://commons.wikimedia.org/wiki/File:Sound_Effects_-_Applause_after_a_concert.ogg) | CC0 1.0 |

Each licence was checked on the track's OWN page, not inferred from the "CC0
Music" collection it appears in — a collection is not a licence.

**Processing applied.** All re-encoded to MP3 at 96 kbps (the crowd at 64 kbps
mono, trimmed to six seconds with a fade), and loudness-matched to −16 LUFS so
no arena is noticeably louder than the next. CC0 permits modification; nothing
here needs to be declared, and the originals remain available at the URLs above.

**Credit is optional but cheap.** CC0 requires none. Section 31 asks for an
optional credit, and a credits screen listing all five authors costs nothing.

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
