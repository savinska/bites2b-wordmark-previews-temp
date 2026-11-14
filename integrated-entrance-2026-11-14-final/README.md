# Bites2B Corrected D2 integrated entrance review

These previews show the integrated first visit experience on the PR #34 marketing surface. The animation ends with the localized slogan and Continue button; the capture then enters the existing homepage.

## Previews

| View | With sound | Silent |
| --- | --- | --- |
| Desktop, 1440 × 900 | `desktop-intro-bg-with-audio.mp4` | `desktop-intro-silent.gif` |
| Mobile viewport, 390 × 844 | `mobile-390-intro-bg-with-audio.mp4` | `mobile-390-intro-silent.gif` |

The standalone silent responsive previews are in `../wordmark-intro-d/`.

## Corrected D2 geometry

The blue 2B paths use a 1.43-unit inward contour offset, not horizontal scaling. Average measured stroke thickness is 56.22 units in Variant D and 53.03 in Corrected D2, a 5.67% reduction. The blue pair is approximately 411.4 units wide and 245.1 units high; its glyphs share a 298.1-unit baseline and retain the 6.9-unit gap. The original SVG viewBox is 1194 × 326.

Coral lettering, the bite, crumbs, brand colors, white background, and enlarged bilingual slogan are retained. Collision geometry is derived from the final paths. Animation choreography and timing are unchanged.

## Sound and licensing

The landing clatter, collision BAM, and bite CRUNCH are synthesized in Web Audio from oscillators, filtered noise, and short envelopes. No third-party recordings, speech, or music are included, so there are no external sound licenses. Playback is initialized only by an explicit user gesture; sound failures do not stop the animation. The final captured audio peaks at approximately −15 dBFS.

## QA

Google Chrome headless was used with desktop and mobile viewport emulation, not physical devices. Both Bulgarian and English were checked at 320, 390, and 1440 CSS pixels. The report records zero page overflow, zero measured layout shift, no runtime/console errors or failed requests, reduced-motion completion state, skip/replay and session behavior, and tenant-route isolation. The existing simulator and guided tour remained available after Continue.

Chromium automation and focused Spring Boot/Thymeleaf and JavaScript tests pass. Safari/WebKit and a physical iPhone were not available in this environment; the captures do not claim real-device verification.
