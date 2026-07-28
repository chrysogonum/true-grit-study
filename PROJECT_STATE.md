# Project State — True Grit Study Tool
*Last updated: 2026-06-29*

## Current Status
A self-contained interactive HTML comprehension tool for Charles Portis's *True Grit* (1968) is built, committed, and deployed live to GitHub Pages. Pitched at a college/advanced reader. Complete and functional.

## Recent Accomplishments (this session)
- Built a single-file HTML study tool (no external dependencies) covering the novel.
- Six tabbed sections: Overview, Plot Walkthrough (8 collapsible "movements"), Characters (with a "triangle of motives" table), Themes & Quotes (4 themes + 5 essay prompts), Vocabulary & Context, and a Self-Test.
- Self-Test has three instant-grading quiz banks (Plot Recall, Detail & Character, Analysis & Theme), each answer explained on submit, with a scaled score message.
- Period-appropriate "parchment" visual design; responsive; sticky tab nav.
- Initialized git repo, created public GitHub repo `chrysogonum/true-grit-study`, pushed `main`, enabled Pages, verified the site returns HTTP 200 with the correct title.

## Known Issues / Blockers
- **Quote accuracy is [UNVERIFIED against a source text in this session].** Quotations were drawn from memory and limited to well-known lines (opening sentence; "Fill your hands, you son of a bitch!"; "You must pay for everything in this world… There is nothing free except the Grace of God."; "Time just gets away from us."). Should be spot-checked against the edition Rehder is using before relying on them.
- The "8 movements" are a pedagogical division; Portis's novel has no numbered/titled chapters. This is disclosed in-tool but worth remembering.
- Repo and Pages site are **public and search-indexable** by design choice this session.

## Key Files
- `index.html` — the deployed tool (served at the Pages root).
- `true-grit-study-tool.html` — identical copy under the original descriptive filename (local convenience copy).
- `PROJECT_STATE.md` — this file.
- `DECISIONS.md` — session decisions (repo visibility, landing-page filename, reading level).

## Live Deployment
- **URL:** https://truegrit.ppr3.com — moved 2026-07-28 from
  `https://chrysogonum.github.io/true-grit-study/`, which now redirects here
- **Repo:** https://github.com/chrysogonum/true-grit-study (public)
- **Branch/source:** `main` / root (`/`); Pages build verified HTTP 200.

## Next Steps
- Verify the four quotations against a physical/known edition; correct if needed and re-push.
- Optional enhancements offered but not yet built: character-relationship diagram, printable study sheet, timeline of the chase.
- If public visibility is undesired long-term, disable Pages or delete/privatize the repo.

## Deployment — recorded 2026-07-28

- **Live site: https://truegrit.ppr3.com** — GitHub Pages, published from branch `main` at the repo root.
- **`git push` IS the deploy.** There is no build step and no wrangler command. Pages rebuilds on
  push and the new bytes are live in about a minute.
- ⚠ GUARD: **do not delete the `CNAME` file at the repo root.** It contains `truegrit.ppr3.com` and is what
  binds the subdomain. GitHub wrote it on 2026-07-28 when the custom domain was set — it was not
  there before, so it can easily read as stray. **Deleting it unbinds the domain** and the site
  falls back to `chrysogonum.github.io/true-grit-study/`.
- The old `chrysogonum.github.io/true-grit-study/` address **301-redirects** here, so links held from before
  the move still work. Verify at `truegrit.ppr3.com`, not at the github.io address.
- ⚠ Because GitHub committed that `CNAME` file itself, the remote moved ahead of local `main`
  without anyone committing. If a push is rejected with `! [rejected] (fetch first)`, rebase onto
  `origin/main` — nothing is wrong.
