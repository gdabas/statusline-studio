# Statusline Studio — memory file

A zero-dependency, single-page web app for designing a Claude Code status line by clicking: compose segments from 65 live-simulated data points, then "Copy for Claude" puts an exact build spec on the clipboard and a target screenshot in Downloads so Claude Code can build and verify the real `~/.claude/statusline.sh`. `README.md` is the full guide (how it works, what is simulated, layout, GitHub Pages deploy). Apache-2.0.

## Shape
- `index.html` (landing), `studio.html` (the app, self-contained, no network calls), `public/` (fonts) — the code. There is no build step.
- `docs/` — `docs/README.md` index plus the demo assets (`demo.gif`, `studio.jpg`) the README embeds.
- `tests/` — `tests/TEST.md` (no automated suite; the manual check is written there).
- `AGENTS.md` — this file; `CLAUDE.md` only imports it (Pagi standard, Sep 10).

## Now
- **State (Sep 10):** released; last change Aug 16 2026 (rate-limit segments show a reset countdown). Deployable as GitHub Pages from the repo root. No automated tests. *(Inferred from git history and the README.)*
- **Last action (Sep 10):** shaped to the Pagi standard — `docs/README.md`, `tests/TEST.md`, this memory file; no code touched.
- **Next:** no owner-stated next step. *Inferred:* keep the simulated data points in step with what Claude Code actually pipes to a status line when that JSON changes.
