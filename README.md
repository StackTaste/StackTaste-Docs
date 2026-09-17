# StackTaste docs

Public docs for [docs.stacktaste.com](https://docs.stacktaste.com). Hosted on [Docs7](https://context7.com/docs7) (Mintlify-compatible).

## Voice

Sentence case. No emoji. No exclamation marks. Short pages: headings, bullets, tables, one code block.

Screenshots only on Quickstart, Dashboard, and Cursor. Put cropped dark-theme PNGs in `images/` when you capture them:

- `images/login-grant.png`
- `images/overview.png`
- `images/taste-list.png`
- `images/agents-cursor.png`

## Preview

From the repo root:

```bash
bun run docs
```

Opens at `http://localhost:3333`. Docs7's preview is a Next.js renderer, so this script uses Node (`npx`), not Bun.

## Host on Docs7

1. Sign in at [context7.com/docs7](https://context7.com/docs7) on the Free plan.
2. Connect this GitHub repository. Point the docs path at `docs/` (`docs.json` lives here).
3. Production branch: the branch you ship (usually `main`).
4. Custom domain: `docs.stacktaste.com` → Docs7 DNS instructions.
5. Each deploy refreshes the Context7 library. `context7.json` at the repo root limits indexing to `docs/`.

You cannot finish DNS or the GitHub OAuth connect from this repo alone. After the first Docs7 project exists, later pushes publish automatically.
