# JASE publication card correction

Date: 2026-11-16 (Asia/Seoul)

Request: remove the visible Published badge, add correct volume and
issue information, and update GitHub.

The existing card reverses the volume and issue as `Vol.9 No.20`.
Correct display: `Vol. 20, No. 9, pp. 1-9`; publication date:
`2026.10.31`. Keep the card's `data-status="published"` so its
publication-count behavior is unchanged. Keep the title and DOI links.

Physical, mathematical, numerical, and fixed-form Fortran changes do
not apply to this HTML metadata update. No Roadmap.md or
master_flowchart.tex was found in the fresh repository inventory.

Sources checked before editing:

- Official journal issue contents:
  https://journal.sase.or.kr/MN/PUBLISH/Main_Publish_list_J2015042.asp
  lists volume 20, issue 9, October 2026, the authors, and the DOI.
- Crossref registration (HTTP 200):
  https://api.crossref.org/works/10.20910/JASE.2026.20.9.1
  returns volume 20, issue 9, pages 1-9, and published date 2026-10-31.
- Independent KCI record checked by the bibliography reviewer:
  https://kci.go.kr/kciportal/ci/sereArticleSearch/ciSereArtiView.kci?sereArticleSearchBean.artiId=ART003397755
  confirms volume 20, issue 9, and pages 1-9.

The network-share checkout is unavailable. Use a fresh clone of
`origin/main` at `b6a79ad` in a dedicated temporary directory.
Do not modify or reset the unavailable original checkout.
Validate the scoped diff, push main, and check the GitHub Pages build
and served HTML. Browser appearance is outside this verification.
