# Aditya & Siddhibala Wedding Invitation

Standalone English website based on source project _1.

- Published URL: https://adityadubey1313-oss.github.io/adisiddhi_1E/
- Language: English only; there is no language switch.
- Features: six schedule entries across 4–6 December 2026, family details and greetings, directions, reception contacts, and WhatsApp sharing. Section order is cover, wedding-day details, complete family section, festivities, venues, and sharing. The existing wedding summary is moved directly below the cover, not duplicated. The family blessing heading and introductory sentence are removed; all family names and greetings remain unchanged.
- Cover: the original `preview.jpg` and dark background treatment carry the Dubey Family invitation, couple names, the cover date of 6 December 2026, and countdown in the first viewport. The displayed festivities span 4–6 December. The remaining sections follow through natural scrolling; no header navigation or opening screen is used.
- Celebrations: Yajnopavita (Janeu) Sanskar, Mandap, Tel-Haldi and Matrika Pooja (4 December, 12:00–5:00 PM); Pushp-Haldi Celebration, Tilak, and Ring Ceremony & Sangeet (5 December, 12:00 PM, 4:00 PM, and 7:30 PM); Barat Wedding Ceremony & Phere and Reception (6 December, 9:00 AM onwards and 7:00 PM onwards). The shared IST note remains applicable to these entries. The 2 December Devi Bhajan and 3 December Mehendi and Magarmaati entries, including their schedule links, are removed.
- Venue evidence: the existing 1E event data explicitly assigns Hotel Gulzar to the 5 December celebrations, wedding ceremony, and reception; these assignments are retained, and the supplied address is used for the 4 December rituals. The obsolete Kishore Kuti card is removed. The separate Hotel Gulzar and Skyway Apartment venue cards are unchanged. The apartment Maps link is an address search, not a verified map pin.
- Family: the exact supplied couple lineage, mother-first parent details, best compliments, and welcoming names appear in the existing family section. The reference image was not attached to this update; wording follows the supplied transcription and existing event-to-venue data.
- Countdown: the existing component updates every second until the reception at `2026-12-06T19:00:00+05:30` and remains at zero afterward.
- Music: one persistent player uses `wedding-song2.mp3`, the same track and two-play behaviour as `adisiddhi_6`. It attempts audible autoplay, plays the track exactly twice, then stops automatically. If blocked by browser policy, a suitable pointer, click, or keyboard interaction retries playback; fallback listeners are removed once playback starts. The fixed top toggle mutes/stops and restarts playback and always reflects the actual audio state. Audible autoplay is browser-controlled and cannot be guaranteed.
- Reception contacts: the existing popup displays the supplied Purushottam Dubey and Saroj Dubey numbers under Family, and the four existing Hotel Gulzar numbers. All six are telephone links; the description is visible.
- Downloads: the calendar button, caption, generation/download code, and standalone `invitation.ics` are removed. Music, directions, contacts, and WhatsApp sharing remain available.
- Assets: relative paths keep this package portable at its repository root.
- Deployment: the repository-local workflow at .github/workflows/deploy-pages.yml publishes this package root to GitHub Pages.

## Automatic scroll nudge

- After a visible page finishes loading, 15 seconds without interaction triggers one 50 CSS pixel downward nudge over 800ms, clamped to available document space. Reloading starts a new visit.
- Touch, pointer presses, clicks, wheel input, keyboard input, focus navigation, manual scrolling, hiding or leaving the page cancel the pending or active hint for that visit. Reduced motion disables it.
- The hint uses native document scrolling without changing content, styling or controls. Run `node --test tests/scroll-nudge.test.cjs` for timing, interaction and lifecycle regressions.

Push this package as the root of its own repository to publish it at the URL above.

Publishing is isolated to `adityadubey1313-oss/adisiddhi_1E` on `main`. Do not push the parent source repository or run bulk-publishing scripts as part of this update. No files belonging to 2E or another version are required.
