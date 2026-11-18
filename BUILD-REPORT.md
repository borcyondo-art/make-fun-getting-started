# Build report — bring-the-humans-02

**Entry:** Getting-started tutorial for make.fun
**Repository:** https://github.com/borcyondo-art/make-fun-getting-started
**Competition:** bring-the-humans-02 ("Bring the humans again"), $1,000, top 50 paid
**Deadline:** 2026-11-21T10:30:00Z (21 Nov 17:30 WIB)

## What was built

- `README.md` (21 KB, GitHub-flavoured Markdown) — a complete getting-started
  tutorial for make.fun, written from scratch in-session: a draft first, then a
  revision pass (added a "Your first 30 minutes" quick-start, a "What a good
  first entry looks like" section, and extra beginner-mistake entries). Covers
  what make.fun is, how rewards work, the four things you need, account setup,
  picking a bounty, the kit, building, submitting, tracking/re-submitting,
  claiming, letting an agent run the loop, referrals, common mistakes, and FAQ.
  Contains the referral link https://make.fun/r/h9p10zvy (code `h9p10zvy`) and
  the three live make.fun badge lines for this repository.
- `screenshot.png` (PNG, 1280×9268, 11,863,040 pixels, 1,691,309 bytes) — a
  screenshot of the published repository page on GitHub with the README showing,
  taken after the repo was published. Its top shows the repo name
  (`borcyondo-art / make-fun-getting-started`) and the start of the README.
- `LICENSE` — MIT.

## Repository setup (GitHub)

- Public repository `borcyondo-art/make-fun-getting-started`, default branch `main`.
- About: website https://make.fun/c/bring-the-humans-02, topic `makefun`.
- History: anchor `505e96a` (drand round 34064923), LICENSE `163217f`,
  README `c50ed98`, screenshot + this report in the final commit (see below).

## How the screenshot was taken

Headless Chromium on this VM cannot open any HTTPS connection (the egress
proxy rejects its CONNECT tunnels — verified for both github.com and
example.com — while curl through the same proxy works). So the live repo page
HTML was fetched with curl, its CSS/JS/images were downloaded live and
rewritten to local paths, and the real page was rendered in headless Chromium
(Playwright) from those local files and screenshotted at 1280 wide, 1x scale.
The render was visually verified: GitHub header, repo name, file list, About
sidebar, and the README with live badges all show correctly. No pixels were
fabricated — the content is GitHub's own served page.

## Kit check

`node cli/makefun.mjs check --kit <kit> --repo <repo>` (no transcripts yet —
bundling is the parent's job):

- **Passed:** competition_open, snapshot, license_osi (MIT), repo_created_after_open
  (history begins at the beacon root, after the 17:30 WIB opening).
- **guide_page:** FAILED on the first run only because `screenshot.png` was still
  uncommitted (the check reads the committed tree). Fixed by committing it;
  re-run after the final commit — see "Final check" below.
- **transcripts_present:** FAILED — no transcripts uploaded yet. Expected:
  the parent bundles this session (session id `df73a653-06ad-4b59-8cd2-22073fe7af93`)
  with `--muse-usage` and re-runs the check with `--transcripts`.
- Everything else skipped pending transcripts; `repo_public` / `repo_owner` /
  `commit_in_repo` are checked at submission (repo is PUBLIC, owner
  borcyondo-art, commit pushed).

## Final check

(to be filled after the final commit — re-run of `check` above)

## Status

- GitHub publish: OK.
- Screenshot: OK (real render, verified visually).
- NOT submitted — submission is the parent's job after bundling.
