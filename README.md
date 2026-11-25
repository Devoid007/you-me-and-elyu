# You, Me & Elyu
A little escape, thoughtfully planned by Radley for Andrea.

## Preview
Open index.html in a modern browser, or serve this folder with `python3 -m http.server 4173 --bind 127.0.0.1` and visit http://127.0.0.1:4173. No Node installation or build step is needed.

## Edit
- config.js: stays, restaurants, itinerary, games, bucket list and dates.
- messages.js: opening letter and ending.
- index.html: headings and supporting copy.
- style.css: visual design and responsive rules.
- coast.svg: original coastal illustration.

Dates are unset. Keep trip.showDates false until public display of dates is separately approved. Set trip.departure to an ISO timestamp with +08:00 only when ready.

Photo pickers store resized photos in this browser using IndexedDB. Notes and preferences use localStorage. Nothing syncs or uploads automatically. Keep originals and export scrapbook notes separately. The share button prepares a summary for the user to send.

## Deployment
Repository: https://github.com/Devoid007/you-me-and-elyu
The repository is private. Do not make it public or deploy the website without Radley’s explicit approval. Once approved, select GitHub Actions as the Pages source, then manually run the Pages workflow. Private-repository Pages hosting may depend on your GitHub plan; confirm available options in settings before changing anything. Every deployed page should be checked on phone and desktop.

The workflow publishes only the explicit static-file allowlist. The private planner is not included in this repository. Never upload it, booking confirmations, precise stay addresses, credentials or private photos.

## Research and QA
See RESEARCH.md, QA.md and PROGRESS.md. Source and mock-DOM logic checks passed locally. The execution environment blocked local server sockets and browser file URLs, so rendered browser and real storage integration checks remain outstanding. Source links, venue hours, host arrival arrangements and prices need reconfirmation for actual trip dates. Unknowns are labeled rather than invented.

The website uses first names only, no analytics, no autoplay, optional motion and noindex/nofollow. Indexing directives are not access control. Fonts load optionally from Google Fonts with local fallbacks. Music uses user-initiated YouTube Music searches.
