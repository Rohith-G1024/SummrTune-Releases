# Changelog

Builds are published here; the source is at
[Rohith-G1024/Summrtune](https://github.com/Rohith-G1024/Summrtune).

The first release describes what the app **does**, rather than what changed —
there is no earlier version to compare it against. Later releases list what
changed.

---

## 1.0.0 — 2026-08-23

The first release with a predecessor, so **this one is a diff**: 0.9.0 went to
one person, and everything below is what changed after they used it.

### New

- **Back up a project to a file, and restore one.** A backup is a single file you
  choose the location for; restoring adds it as a new project and never touches
  what you already have. Back up from a project's ⋯ menu, restore from
  **Settings → Storage**.
- **Convert a stereo track to mono.** A stereo track cannot use EQ, the
  compressor, the de-esser, delay, reverb, fade, pitch correction or vocal
  transpose — all of those need one voice. Converting unlocks them. It is in
  the track's ⋮ menu on the timeline, it asks first, and **it cannot be
  undone**: the two channels are folded into one for good, so anything wide can
  thin out.
- **Three more colour families**, taking the set to nine: *Cobalt* (deep water
  and gold), *Honey* (burnt honeycomb and bright yellow) and *Guava* (rind green
  and melon).
- **Track colours now follow the colour family.** Every family has its own twelve,
  solved from that family's own accent and warning colours.
- **Colour is offered on every track**, including the anchor and both halves of a
  separation, with a *neutral* option to go back.
- **Duplicate a track**, from the track menu.
- **Check for updates by hand**, in **Settings → Updates** — the one place a
  failed check says so.
- **The update notice can be turned off from the notice itself.** *Don't ask
  again* switches off the same *Auto-check* setting Settings shows, so the two
  can never disagree; the × still means *not now*, and the next release is
  offered again.
- **Punch in over an existing track** without creating a new one.
- **Import from the timeline**, with a `+` row at the end of the track list.
- **The piano keys play their note**, in the song's own tuning rather than
  concert pitch.

### Changed

- **Every tab's title bar is the same component** — same height, same position,
  same corner menu — so switching tabs no longer moves the page.
- **Settings buttons now mean something by how they look**: solid is *press
  this*, an outline is a door, a red outline deletes.
- **The anchor track reorders like any other.**
- ***Free up space* now leaves the layer's own audio as its original**, so a
  track is never left pointing at something that is gone.
- **A greyed-out effect opens read-only**, so the explanation for why it is
  greyed is reachable.
- ***Clear pitch correction settings* is now *Default settings***, on all three
  arms.
- The Recording screen's *Starts at…* line moved to the row above the transport,
  beside the numbers it is about.
- Preset cards no longer print *untested*.

### Fixed

- **Deleting the original of a duplicated track destroyed the copy's audio.**
  This was data loss and it is the most important line here. Audio already lost
  cannot be recovered.
- **A trimmed track re-applied its effects on the next save.**
- **Pitch correction ran a full pass on tracks it would not change**, captioning
  a save *Tuning* when nothing was being tuned.
- **The Amount slider on a scoped effect read one region and wrote the whole
  track.**
- **Reverb could not be opened on a stereo track**, which hid its own
  explanation.
- **A menu opened under the wrong end of its row.**
- **Punching in before a track's audio started** placed the recording wrongly.

---

---

## 0.9.0 — 2026-08-21

The first build that leaves the developer's phone. Feature-complete for what 1.0
is meant to be; **0.9.0 rather than 1.0 because it has not been run by anyone
else yet** — what is being withheld is confidence, not features.

### Record

- Sing over a backing track and stack up to **eight tracks** on one timeline.
- A take starts **at the playhead**, not at zero, and everything else plays while
  you sing.
- Choose your microphone and your headphones **independently**; the choice is
  remembered per app, including while the device is unplugged.
- The round-trip delay of your route is compensated automatically, and takes can
  be nudged by hand when it is not quite right.
- Listen back to a take before you keep it. Nothing joins the project until you
  say so.
- Ten-minute cap on anything recorded or imported.

### Split a song into its parts

- Pull the singing away from the music, or the other way round, entirely on the
  phone — **no upload and no account**.
- Both halves arrive as tracks, the one you asked for playing and the other kept
  muted.
- **Nothing shifts in time**, so takes recorded against the original still line
  up.
- Runs in the background with the screen off.

### Fix and shape a take

- **Noise removal** — hiss, hum and room sound, with the gaps between lines
  gated.
- **Pitch correction** — key-locked, from a gentle repair through to the hard
  tuned sound, with a keyboard for picking notes by hand.
- **Detect key and tuning** — works out the key from your voice and what the song
  is tuned to from the backing track, and fills both in.
- **Silence** — wipe a cough or a false start out of the middle of a good take.
- **Level** — measures how loud you actually sang and suggests a matching volume.
- **Transpose and key change** — move your voice, or change the key of the whole
  backing track while it plays.
- **EQ, compressor, de-esser, delay, reverb and fade**, all instant: move a
  control and the change is in what you hear.
- **Every effect can be pointed at part of a track** rather than all of it — up
  to eight stretches, each with its own settings.
- **Preview** renders exactly what saving would give you and plays it without
  keeping it, so you can compare before you commit.
- **Restore original audio** takes any track back to how it arrived.

### Mix and export

- Volume, pan and mute per track, plus a master fader and a safety limiter that
  stops the mix clipping.
- Export to **WAV** or **M4A**, named and placed where you choose, defaulting to
  a SummrTune folder in your music library.
- What you export is exactly what you hear.

### Around the edges

- **Six colour schemes** over three families, each in light and dark.
- A **guide** covering every part of the app, reachable from Settings and from a
  `?` beside the controls that need one.
- A **diagnostic report** you can read in full and send yourself — names replaced
  with short codes, and no audio, ever.
- An **update notice**: once a day the app asks the release page whether a newer
  version exists, and says so if there is one. That is the only thing it ever
  sends or asks for, it can be switched off, and it never downloads or installs
  anything — the notice opens the page in your browser and you decide.
- **Works entirely offline.** No account, no cloud, no telemetry.

### Known limits

- Requires Android 11 or newer, on a 64-bit ARM phone.
- The app is **182 MB** installed, most of which is the two separation models —
  they ship inside the app so that splitting a song never needs the internet.
- Uninstalling deletes every project. Export anything you want to keep.
