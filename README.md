# IDEX Security Academy

Interactive, English-language employee learning pilot. Buildless HTML, CSS and JavaScript; deploy `dist/`.

## Features

- Eight missions with 24 fictional decisions. Six missions focus on IDEX products and the identity / access lifecycle; two cover everyday security and response.
- Feedback, primary-source links, local progress, XP without repeat-answer farming and four learning badges.
- Digital / physical card lab with independent identity-assurance, user-verification and authorisation conditions.
- Six-question practice challenge, searchable glossary and a downloadable self-directed learning record.
- Responsive navigation, visible keyboard focus, accessible form controls and reduced-motion support.

## Data

The app makes no external API calls. It stores question mastery, attempt count, earned XP and the best challenge score in localStorage under `idex-academy-v1`. This is not a centrally verified training record. The host may independently keep access logs. No biometric data is collected. There is no real hardware authentication.

## Content maintenance

Edit `dist/content.js` for mission content and source references. Content was checked against public IDEX Help Centre / product pages, FIDO Alliance, UK NCSC and Microsoft documentation on 2 November 2026. Generic AI handling guidance is adapted as a general principle, not asserted as IDEX policy. Scenarios are original fiction, not incident reports or approved company procedures.

Before employee rollout, the product/security owners must verify profile-specific behaviour and add the actual incident / lost-card reporting route, policy links, visitor process and approved tools. This private pilot has no LMS, SSO, employee directory, email sending, real phishing simulation or central manager reporting. Sharing is managed separately by Sites.

## Verification

`node --check dist/app.js` and `node --check dist/content.js` verify JavaScript parsing. UI verification should cover mission completion, retry scoring, reload persistence, non-farming replay, challenge scoring, all lab conditions, glossary search, export and reset. Use the Sites managed preview for browser QA.
