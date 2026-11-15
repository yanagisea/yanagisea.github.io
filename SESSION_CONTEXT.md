# Session context

## 2026-11-15: MDPI Aerospace publication

- Request: remove the review tag and display/link DOI
  `10.3390/aerospace13111069` for the published paper.
- Basis recorded before implementation in `docs/publication_update.md`
  and `docs/publication_update.tex`.
- Target: the MDPI Aerospace card in `index.html`.
- Update the status to published so the existing publication counter
  includes the paper. Link the title and visible DOI.
- Follow-up request: externally verify and display the volume and issue.
- MDPI official issue contents confirm `Aerospace 2026, 13(11), 1069`
  and publication date `15 November 2026`. Publisher PDF first-page
  text also confirms the title, DOI, volume, article number, and date.
  Full source links and verification limits are in the basis documents.
- Display `Vol. 13, No. 11, Article 1069` and `2026.11.15`.
- The MDPI contents label the DOI `registering DOI`; Crossref and
  doi.org returned 404. The two checked documents share one publisher,
  so independent two-source verification is not claimed.
- Initial untracked files: `papers/index.html` and
  `yanagisea.github.io.code-workspace`. Preserve both.
- No Roadmap.md or master_flowchart.tex was found in the initial inventory.
- Validation: `git diff --check` passed. Node assertions passed for the
  published status, removal of the review badge, volume/issue/article,
  publication date, both DOI links, and eligibility for the existing
  publication counter. Browser rendering was not checked.
- No commit, push, or deployment performed.

## 2026-11-15: GitHub update request

- The user authorized committing and pushing the publication and profile
  typography changes to GitHub.
- Target: `origin/main` in `yanagisea/yanagisea.github.io`.
- `git fetch origin` completed; HEAD and origin/main both start at
  `710636e`, with no divergence before this update.
- Scope: `index.html`, this context file, and the four task basis
  documents in `docs/`. Preserve the two pre-existing untracked files.
- Pre-push diff review and `git diff --check` passed. The prior browser
  rendering limitation remains; no visual deployment acceptance is claimed.
- This entry records the release scope before commit. Push and remote
  verification results will be reported in the session response.

## 2026-11-15: Profile name typography

- Request: modernize the top card's Hangul and kanji font.
- The two name/pen-name rows are the only users of `.serif`.
- Basis recorded before editing in `docs/profile_typography.md` and
  `docs/profile_typography.tex`, with primary font/API references.
- Use scoped Noto Sans KR / Noto Sans JP stacks, explicit Korean and
  Japanese language tags, normal spacing, and an upright pen-name label.
- Keep names, ruby readings, and the earlier publication changes.
- Validation: `git diff --check` passed. The Google Fonts CSS request
  returned HTTP 200 and declared Inter, JetBrains Mono, Noto Sans JP,
  and Noto Sans KR. Source/diff review confirms scoped font rules and
  preserved name/ruby text and publication edits.
- Browser preview could not be checked: browser inventory reported
  `The browser access host is unavailable`; native fallback returned
  `GetCursorPos failed` with `0x80070005` (access denied).
- No commit, push, or deployment performed.
