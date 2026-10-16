# Blair's Career Quest: Cloud Architect Chronicles

**An interactive career RPG by Blair Page**

A fully playable, free-to-host browser game that transforms a technical résumé into an explorable world. Visit six career realms, solve five fictional infrastructure incidents, explore a skill tree, view professional training, and switch instantly to Recruiter Mode.

## Play

After enabling GitHub Pages, open `https://blairyfairy.github.io/Blairs-Career-Quest/` (assuming this repository is named `Blairs-Career-Quest`).

**Controls:** WASD / arrow keys to move; **E** or **Space** near a realm to enter. Click or tap portals directly. Touch movement buttons are included. Use the top navigation to open Missions, Skill Tree, Achievements, or Recruiter Mode without playing.

## Features

- Original canvas-rendered 2D explorable map, with six career-themed realms
- Five interactive incident-response scenarios with explanations
- Mission completion tracking stored locally in the browser
- Technical skill tree with technologies sourced from the professional portfolio
- Achievement vault pointing back to credential evidence
- Recruiter Mode with work-history summary and direct ATS / portfolio links
- Mobile-responsive layout, accessible navigation, optional synthesized audio
- Zero build steps, zero external runtime dependencies, no analytics or API keys

## Deploy to GitHub Pages (free)

1. Create a **public** repository called `Blairs-Career-Quest` on GitHub.
2. Upload the contents of this folder **at the repository root**, including `index.html`, `style.css`, `data.js`, and `game.js`.
3. Open **Settings → Pages → Build and deployment**. Select **Deploy from a branch**, branch **main**, folder **/(root)**, and save.
4. Once GitHub completes deployment, visit `https://blairyfairy.github.io/Blairs-Career-Quest/`.
5. Optionally add the game URL to the main Blair Page portfolio and LinkedIn Featured section.

The game also works by opening `index.html` locally in a browser. It can be hosted on Cloudflare Pages, Netlify, or itch.io as a static HTML game.

## Customize

- `data.js` — six realms, job entries, credential summaries, and mission scenarios.
- `style.css` — color palette, typography, responsive layout.
- `game.js` — world map, input controls, quest logic, progress storage, navigation.
- `index.html` — page structure, metadata, external portfolio links.

For new missions, append an object with a unique `id`, `realm`, `title`, `level`, `story`, three `answers`, zero-based `correct` index, and `why` explanation to `CAREER.missions` in `data.js`.

## Accuracy and provenance

The career descriptions were adapted from Blair Page's supplied professional portfolio snapshot dated October 16, 2026. See [`docs/SOURCE_NOTES.md`](docs/SOURCE_NOTES.md). The incidents are **fictional educational exercises**, not claims about actual employers, customers, or live systems. The game awards **local in-game mission completion only**; it does not confer professional credentials. Credential verification remains on the linked original portfolio / issuers.

## Privacy

No accounts, tracking, or remote databases. Mission completion is saved only in the visitor's browser `localStorage`; the reset button clears it. The game uses no cookies, telemetry, or third-party scripts.

## Credits and license

Project branding and career profile: **Blair Page**. Game implementation is included as editable source files. This package was prepared with AI assistance from ChatGPT; review and customize before representing the code as solely human-written. No third-party art, audio, or font files are required.

MIT License — see [LICENSE](LICENSE).
