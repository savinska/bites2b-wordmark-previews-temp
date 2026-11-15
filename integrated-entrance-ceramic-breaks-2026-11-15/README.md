# Bites2B ceramic plate-break intro review

These MP4s contain actual audio captured from Chromium's Web Audio output. Video is H.264 and audio is AAC.

## Play previews

- [Full desktop, 1440 × 900, with audio](desktop-intro-bg-with-audio.mp4)
- [Full mobile viewport, 390 × 844, with audio](mobile-390-intro-bg-with-audio.mp4)
- [Opening 1.8 seconds, ceramic plate breaks only](desktop-falling-letters-first-1-8s-with-audio.mp4)
- [Captured audio waveform](audio-waveform.png)

## Mix verification

[RMS/peak levels, prior-preview comparison, timing and BAM gain](audio-levels.json). Across the combined AAC mix, plate section (0.5–1.5 s) measured −22.28 dBFS RMS / −6.60 dBFS sample peak on desktop and −22.23 / −7.31 dBFS in the mobile viewport. BAM (2.1–2.6 s) measured −15.99 / −2.44 desktop and −15.99 / −2.45 mobile. CRUNCH (3.3–4.0 s) measured −26.39 / −3.42 desktop and −26.30 / −3.08 mobile. BAM gain is 1.17 versus 0.88 previously (+2.47 dB); master remains 0.82. BAM and CRUNCH source assets are unchanged, as are CRUNCH time and gain.

Five distinct genuine ceramic plate-break recordings are used, with CC0 1.0 licenses, exact source pages, author names, trim lengths, and pitch variation documented in [SOURCES.md](SOURCES.md). All cafeteria ambience, conversation, cutlery, and plate-stack cues were removed. Browser QA verified muted mode and audio-load failure fallback; see [browser-qa.json](browser-qa.json). Mobile is viewport emulation, not an iPhone speaker recording.
