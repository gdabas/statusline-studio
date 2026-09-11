# Tests — Statusline Studio

There is no automated test suite; the app is a single self-contained HTML file with no build step.

**Manual check (the one that matters):** open `studio.html`, compose a two-row status line, press *Copy for Claude*, and confirm the clipboard holds the spec and `statusline-target.png` landed in Downloads; then paste into Claude Code and confirm its rendering matches the screenshot. Clipboard APIs need `https://` or `http://localhost` (`python3 -m http.server 8080`).

Last observed: not run on Sep 10 2026. If a browser test is added (Playwright would fit), put it under `tests/` and record the command here.
