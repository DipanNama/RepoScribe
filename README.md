# RepoScribe

A local-first naming workspace: describe a project, choose type/tone and get six repository-name directions, descriptions and tags. Copy names/all results, export JSON, clear and switch theme. Live browser demo and permission-free Chrome popup ZIP.

## Honest first release

This is rule-based, deterministic local generation, not AI. No account, API key, upload, availability/trademark check or automatic repository creation. The original AI vision is future work; names are starting points, not unique/available guarantees. Only theme is saved. User input renders as text, never HTML.

## Development

Node 22 and system zip: `npm test` (14 unit tests), `npm run build`. Serve `dist` with a static server. No npm installation needed. The workflow deploys dist only. Browser tests cover generation, tone, copy feedback, safe text rendering, invalid brief, JSON export, reset, persisted theme, mobile overflow and popup UI. Output is self-contained and works offline once loaded.

## Chrome popup

Download reposcribe-extension.zip from the live demo, unzip it, open chrome://extensions, enable Developer Mode, choose Load unpacked and select the extracted folder. No permissions, content scripts, host access, background worker or API keys. It is not published in the Chrome Web Store. The same external JS runs under Manifest V3 CSP; the popup is separately tested locally.

## Release workflow

Work on a typed branch, test/build locally and inspect desktop dark/mobile. One PR/squash to main triggers Production Pages once. Only main pushes build; no branch/PR/tag/manual trigger. Pages Source Actions and github-pages environment main-only before merge.

## Sources

Buttons adapted from Pines: https://devdojo.com/pines/docs/button . Component discovery: https://shoogle.dev/ . Icons embedded locally from Lucide (ISC), see LICENSE-icons. No remote scripts/fonts/assets. Existing repository license was referenced but absent, so this release does not invent a project license grant.

Roadmap: AI generation through a securely configured backend, explicit GitHub availability checks, banners and optional repository creation with separate authorization.
