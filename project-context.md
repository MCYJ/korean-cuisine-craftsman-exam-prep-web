# KOR-0172 marketing site context

## Scope

- Independent public marketing and study site for released app `KOR-0172` only.
- App source is read-only: `/Users/youngjunma/Documents/various test prep apps project/services/kor/01/kor-0172`.
- Android package and iOS bundle identifier: `app.mcyj.examprep.kor0172`.
- Production target: `https://mcyj.github.io/korean-cuisine-craftsman-exam-prep-web/`.

## Verified Store state — 2026-09-19

- Google Play resolves publicly for the exact package.
- Apple lookup resolves the exact bundle to track ID `6797324369` in the KR storefront.
- Both official Store badges are active and use the same 194 × 75 px outer frame without distorting artwork.

## Content and official facts

- Korean and English routes with 10 substantive guides per locale.
- Official name: 한식조리기능사 / Craftsman Cook, Korean Food (`jmCd=7910`).
- Written: four-option multiple choice, 60 items in 60 minutes; pass mark 60/100.
- Practical: cooking work from requirements and supplied ingredients; pass mark 60/100. Task-specific time must be checked in the current public task.
- Q-Net identifies hygiene and safety, cooking technique and finished-work quality as major practical evaluation areas.
- The official 2026 public-task post was registered 2025-12-24 and applies from the first 2026 continuous practical exam. It includes the task status, change history, hygiene/safety criteria and public-task archive.
- Canonical sources:
  - `https://www.q-net.or.kr/crf005.do?id=crf00503&jmCd=7910`
  - `https://www.q-net.or.kr/crf005.do?id=crf00503s02&jmCd=7910&jmInfoDivCcd=B0`
  - `https://www.q-net.or.kr/cst006.do?artlSeq=5250945&brdId=Q006&code=1204&gId=&gSite=Q&id=cst00602`
  - `https://www.q-net.or.kr/rcv013.do?gSite=Q&id=rcv01306s02&jmCd=7910`

## Design and implementation

- Visual thesis: bright kitchen cream, olive preparation surfaces and restrained red accents, with a prep–cut–cook–plate workflow.
- Global Korean-safe wrapping uses `word-break: keep-all` and `overflow-wrap: break-word`.
- Dependency-free static generator; GitHub Actions builds, checks and deploys `dist/` to Pages.

## Verification log

- 2026-09-19: project initialized from the proven static-site system and fully retargeted to KOR-0172 content, assets and Store identities.
- 2026-09-19: local build generated 34 indexable routes and 36 HTML files total; the site checker passed metadata, links, exact Store identities, `keep-all` and equal badge frames.
- 2026-09-19: local HTTP QA returned 200 for all 34 sitemap routes and five key assets; an unknown route returned 404.
- 2026-09-19: live Store recheck returned Google Play 200 and Apple bundle `app.mcyj.examprep.kor0172`, track ID `6797324369`.
- 2026-09-19: GitHub Pages workflow run `35362069829` completed successfully.
- 2026-09-19: production QA returned 200 for all 34 sitemap routes and five key assets; an unknown route returned 404.
- 2026-09-19: production CSS contains global `word-break: keep-all` and the shared 194 × 75 px marketplace frame; the Korean home contains both exact public Store links.
