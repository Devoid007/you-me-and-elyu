# QA results

## Passed in this session
- JavaScriptCore syntax parsing of website configuration, messages and application.
- App logic executed against a mock DOM: accommodation selection and local persistence, recommendation context, food randomizer excluding unverified leads, question category and reroll, dice selection / decline, mood preferences, bucket progress, share summary, escaping, storage failure and final confirmation.
- HTML parser checks: unique static IDs, valid internal anchors, all script and image references exist.
- Public artifact checks: first names only, no precise travel dates or stay addresses / private planner links, indexing directives, no autoplay or embedded tracking frames, reduced-motion CSS.
- Private planner JavaScript syntax and expense logic checked separately.
- GitHub Pages workflow uses a fixed public file allowlist and a manual dispatch trigger; no publication occurred.

## Not verified here
The environment denied a local listening socket; browser file URLs are disallowed. Therefore no rendered browser QA, screenshots, actual localStorage / IndexedDB integration, image picking, Web Share / clipboard permissions, font loading, external-link reachability, console audit or production verification was completed. Mock DOM tests do not establish browser correctness.

## Required browser acceptance checks
Use a modern browser on localhost, then test widths 320, 375, 390, 430, 768, 1024 and 1440 pixels. Check no horizontal overflow, readable type, keyboard focus and envelope trapping, menu, every button, compare table scroll, selection reload, mood reload, dice, all question categories, checklists, photo upload/reload/remove, export, share fallback and motion preference. Test private planner invalid / zero inputs and total calculation. Confirm no console errors. Run with blocked storage and reduced-motion enabled. Inspect mobile Safari as well as desktop Chromium. Verify all source, Maps and music links manually.

## Build / tooling
No build is required. Node, npm and GitHub CLI are absent; terminal outbound DNS is restricted. React / TypeScript lint and build checks do not apply to this dependency-free implementation. See README for the deliberate stack deviation and deployment steps.
