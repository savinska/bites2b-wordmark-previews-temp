# BAM A/B review

These desktop and mobile MP4s are full browser captures with the actual Web Audio output. Visuals, animation choreography, BAM event time and per-event gain, ceramic plate clips and gains, CRUNCH file, time and gain are the same in both versions.

## Play

| Version | Desktop, 1440 × 900 | Mobile viewport, 390 × 844 |
| --- | --- | --- |
| A — restrained body and onset | [Play MP4](desktop-bam-a-with-audio.mp4) | [Play MP4](mobile-390-bam-a-with-audio.mp4) |
| B — deeper tone and stronger onset | [Play MP4](desktop-bam-b-with-audio.mp4) | [Play MP4](mobile-390-bam-b-with-audio.mp4) |

[A/B waveform](bam-ab-waveform.png) · [Full measurements and source hashes](audio-levels.json) · [Browser QA](browser-qa.json) · [Sound source and processing notes](SOURCES.md)

## Measurements

Combined browser AAC levels, RMS / sample peak in dBFS:

| Capture | Version | Ceramic plates, 0.5–1.5 s | BAM, 2.1–2.6 s | CRUNCH, 3.3–4.0 s |
| --- | --- | --- | --- | --- |
| Desktop | Prior | −22.28 / −6.60 | −15.99 / −2.44 | −26.39 / −3.42 |
| Desktop | A | −22.28 / −6.60 | −16.04 / −2.50 | −26.39 / −3.42 |
| Desktop | B | −22.24 / −6.41 | −13.45 / −1.45 | −26.40 / −3.51 |
| Mobile viewport | Prior | −22.23 / −7.31 | −15.99 / −2.45 | −26.30 / −3.08 |
| Mobile viewport | A | −22.24 / −7.31 | −16.10 / −2.49 | −26.31 / −3.08 |
| Mobile viewport | B | −22.28 / −6.41 | −13.61 / −1.75 | −26.36 / −3.49 |

B raises the measured BAM about 2.5 dB RMS / 1 dB sample peak on desktop and 2.4 dB RMS / 0.7 dB peak on mobile, staying below 0 dBFS. A is within about 0.1 dB of the prior BAM mix. A's source is the same approved take with moderate 140 Hz body lift and a brief onset emphasis. B uses that same take, lowered 0.89 semitones with a stronger 105 Hz/body emphasis, onset lift, and shorter tail. The approved CRUNCH source hash, schedule and gain are unchanged; tiny AAC peak differences are encoder variation.

There is about 0.40 s between the final ceramic cue's end and the BAM. Their tails do not overlap, so no plate ducking was applied. Both retain the same 2.13 s BAM timing and 1.17 event gain; master gain remains 0.82.

The mobile captures use a 390 × 844 Chromium viewport emulation, not a physical iPhone. Safari/WebKit was unavailable.
