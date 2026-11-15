# Bites2B Corrected D2 integrated entrance review

These previews show the integrated first visit experience on the PR #34 marketing surface. The animation ends with the localized slogan and Continue button; the capture then enters the existing homepage. MP4 files contain the actual local recorded intro audio and use H.264/AAC for mobile playback.

## Previews

| View | With sound | Silent |
| --- | --- | --- |
| Desktop, 1440 × 900 | [MP4 with audio](desktop-intro-bg-with-audio.mp4) | [Silent GIF](desktop-intro-silent.gif) |
| Mobile viewport, 390 × 844 | [MP4 with audio](mobile-390-intro-bg-with-audio.mp4) | [Silent GIF](mobile-390-intro-silent.gif) |

[First 1.8 seconds with audio (falling-letter sound check)](desktop-falling-letters-first-1-8s-with-audio.mp4) · [Audio level comparison](audio-levels.json)

The standalone silent responsive previews are in [Corrected D2 standalone](../../corrected-d2-standalone-2026-11-14/).

## Corrected D2 geometry

The blue 2B paths use a 1.43-unit inward contour offset, not horizontal scaling. Average measured stroke thickness is 56.22 units in Variant D and 53.03 in Corrected D2, a 5.67% reduction. The blue pair is approximately 411.4 units wide and 245.1 units high; its glyphs share a 298.1-unit baseline and retain the 6.9-unit gap. The original SVG viewBox is 1194 × 326.

Coral lettering, the bite, crumbs, brand colors, white background, and enlarged bilingual slogan are retained. Collision geometry is derived from the final paths. Animation choreography and timing are unchanged.

## Sound and licensing

The soundscape uses licensed recordings: a public-domain restaurant ambience bed, CC0 porcelain plate stacking, public-domain cutlery placement, a public-domain dull thud for the single collision BAM, and a CC0 crispy-toast bite for the CRUNCH. Trim details, authors, and license links are documented in [SOURCES.md](SOURCES.md). No speech, music, electronic effects, or synthesized substitutes are used. Audio is decoded after the visitor explicitly enables sound; cues are scheduled against the existing letter landing, collision (`T.contact`), and bite (`T.bite`) animation times. Ambience fades to silence before the bite. Audio failure leaves the animation silent and usable.

The opening mix now uses audible plate excerpts from active parts of the source recording and distinct cutlery-placement transients. The cafeteria layer rises to 0.72 gain during the falls (12 dB above the previous 0.18 level) and fades back to its previous 0.085 level by the 2B contact. Plate and cutlery event gains are set separately; the master, BAM, and CRUNCH gains are unchanged. In the exported desktop recording, the 0.5–1.5 s window improved from −42.2 to −21.5 dBFS RMS (+20.7 dB); the 2.1–2.6 s collision window and 3.3–4.0 s bite window measured the same as before to 0.1 dB. The maximum sample peak in the falling window is −4.6 dBFS. See [the isolated first 1.8 seconds](desktop-falling-letters-first-1-8s-with-audio.mp4) and the full [desktop/mobile waveform comparison](audio-levels.json).

## QA

Google Chrome headless was used with desktop and mobile viewport emulation, not physical devices. Both Bulgarian and English were checked at 320, 390, and 1440 CSS pixels. The report records zero page overflow, zero measured layout shift, no runtime/console errors or failed requests, reduced-motion completion state, skip/replay and session behavior, and tenant-route isolation. AudioContext was running and the browser recorded actual audio in both previews. The existing simulator and guided tour remained available after Continue.

Chromium automation and focused Spring Boot/Thymeleaf and JavaScript tests pass. Safari/WebKit and a physical iPhone were not available in this environment; the captures do not claim real-device verification. The MP4 previews are intended for iPhone review, but native iOS Safari playback still needs a real-device check.
