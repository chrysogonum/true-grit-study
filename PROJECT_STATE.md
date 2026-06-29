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
- **URL:** https://chrysogonum.github.io/true-grit-study/
- **Repo:** https://github.com/chrysogonum/true-grit-study (public)
- **Branch/source:** `main` / root (`/`); Pages build verified HTTP 200.

## Next Steps
- Verify the four quotations against a physical/known edition; correct if needed and re-push.
- Optional enhancements offered but not yet built: character-relationship diagram, printable study sheet, timeline of the chase.
- If public visibility is undesired long-term, disable Pages or delete/privatize the repo.
