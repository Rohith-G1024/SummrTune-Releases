# SummrTune

A pocket recording studio for singing. Record covers over a backing track, stack
harmonies, clean up the recording, fix the tuning, and save a finished song —
**all on the phone**, with no account, no cloud, and no internet required.

**[Download the latest version](https://github.com/Rohith-G1024/SummrTune-Releases/releases/latest)**

This repository carries the builds. The source lives at
[Rohith-G1024/Summrtune](https://github.com/Rohith-G1024/Summrtune).

---

## What it does

- **Record** over a backing track, up to eight tracks in one song. A take starts
  wherever the playhead is, and everything else plays while you sing.
- **Split a song** into the singing and the music, on the phone, so you can sing
  over the instrumental of anything you own.
- **Clean up and tune** — noise removal, pitch correction with automatic key and
  tuning detection, silence out a cough, transpose a song into your range.
- **Shape it** — EQ, compressor, de-esser, delay, reverb and fades, all of which
  change what you hear the moment you move them.
- **Save it** as a WAV or an M4A, wherever you want it.

## Installing

The app is not on the Play Store. Download the `.apk` from the
[latest release](https://github.com/Rohith-G1024/SummrTune-Releases/releases/latest)
and open it; Android will ask whether to allow installing from your browser.

**Requirements**

| | |
|---|---|
| Android | 11 or newer |
| Phone | 64-bit ARM (any phone from the last several years) |
| Space | about 400 MB to install, and more for your recordings |

The download is large — around 180 MB — because the models that split a song into
its parts ship **inside the app**. That is what lets it work with no internet and
send nothing anywhere.

## Privacy

Nothing you record, import or make ever leaves your phone. There is no account,
no cloud, no backup and no analytics.

The app makes **one** kind of network request: once a day it asks this repository
whether a newer version exists, so it can tell you. It sends nothing about you
when it asks, it never downloads or installs anything by itself, and you can turn
it off in Settings. Everything works with it off, and with the internet off.

**Because there is no cloud, there is no backup.** Uninstalling deletes your
projects. Export anything you want to keep.

## Reporting a problem

Settings → Diagnostics builds a text report describing your phone, your audio
setup and what the app was doing. You see the whole thing before anything
happens, project and file names appear only as short codes, and no audio is ever
included. Nothing is sent automatically — the app hands you the file and you
choose what to do with it.

Send it, along with what you were doing, to
[Issues](https://github.com/Rohith-G1024/Summrtune/issues).

## Changelog

[CHANGELOG.md](CHANGELOG.md).
