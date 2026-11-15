# Profile typography basis

Date: 2026-11-15 (Asia/Seoul)

Request: modernize the Hangul and kanji font in the top profile card.
The two name/pen-name rows currently use Noto Serif KR. No other row
uses that font class.

Use Noto Sans KR for Korean and Noto Sans JP for Japanese kanji and
kana, with Inter for Latin characters and system sans-serif fallbacks.
Mark the Korean rows and Japanese runs with their language tags so
Japanese names use the appropriate font. Keep ruby readings and text.
Remove the wide tracking and the pen-name label's font override/italic.
Scope the CSS to these two rows.

This is a visual CSS/HTML change. Physical, mathematical, numerical,
and fixed-form Fortran implementation requirements do not apply.
No Roadmap.md or master_flowchart.tex is present in the repository inventory.

Primary references checked before implementation:

- Noto CJK project: https://github.com/notofonts/noto-cjk
  documents the Sans families and Japanese/Korean regional versions.
- Google Fonts CSS API: https://developers.google.com/fonts/docs/css2
  documents requests for multiple families and selected weights.

Verification: inspect the local browser preview and the scoped diff.
Preserve the earlier publication update and existing untracked files.

Result: `git diff --check` passed. Google Fonts returned HTTP 200 with
all four requested font families. Source review confirms that both rows
use the new stacks, preserve names/readings, and have normal tracking.
Browser rendering was not verified: the browser access host was unavailable
and native fallback failed with access denied (`0x80070005`).
No commit, push, or deployment was performed.
