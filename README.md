# Write skills like procedures

Talk deck: Simplified Technical English for agent skills. Built on a Vite + [reveal.js](https://revealjs.com/) scaffold.

**Live deck:** [https://jrabbott.github.io/talk-write-skills-like-procedures/](https://jrabbott.github.io/talk-write-skills-like-procedures/)

## Talk in one sentence

Agent skills are procedures, not prompt poetry — write them with STE-shaped clarity so the agent can’t misunderstand the next action.

## Requirements & run locally

- **Node.js 22+** (see `.nvmrc`). Prefer `npm ci` so the lockfile is respected.

```bash
npm ci
npm run dev
```

Open the URL Vite prints (usually `http://localhost:5173/talk-write-skills-like-procedures/`).

To check the production build:

```bash
npm run build
npm run preview
```

## Present

1. Start with `npm run dev` (or open the live Pages URL).
2. Click the slides, then use arrow keys / space to navigate.
3. Press `F` for fullscreen, `S` for speaker notes, `Esc` for overview.
4. After the CTA, paste [`cheat-sheet.md`](cheat-sheet.md) into chat.

Speaker notes live in `<aside class="notes">`. Treat them as trusted HTML only.

## Deck outline

- Title — Write skills like procedures
- Personal open — dyslexia → LLMs → STE → how it helps read & write → thesis
- STE → skill mapping — four conventions; anti-patterns in one breath
- Before/after — Example A (vague verbs); Example C (nested conditionals); synthetic only
- Risks — too rigid; keep exact tokens; no full STE checker yet
- CTA — rewrite one skill’s Steps + Do not; cheat sheet in chat
- Stretch (to 25) — Example B, Example D, anti-pattern table, Q&A hold

Author outline: [`docs/outline.md`](docs/outline.md). Handout: [`cheat-sheet.md`](cheat-sheet.md).

## Pages

After merge: **Settings → Pages → Build and deployment → Source: GitHub Actions** (if not already set).

## License

[MIT](LICENSE) © 2026 Jon Abbott
