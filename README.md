# LXP El Salvador 2026 — Rubric v7.4

Interactive browser for the LXP procurement evaluation rubric used by the World Bank LAC Education team to assess three platforms proposed for national deployment in El Salvador:

- **IHFB** (Korean cooperation donation)
- **Kira Learning** (Andrew Ng + Anthropic)
- **Grok** (xAI, in negotiation with the Salvadoran government)

## What this is

The rubric has **14 pedagogical domains** broken into **98 cells**, with a maximum score of **116 points** and a procurement-grade threshold of **60% (≥70 pts)**. Each cell is scored PASS / PARTIAL / FAIL / N/A with traceable evidence.

This static site lets you:

- Browse all 98 cells with search, filter (domain, severity, platform, status), and deep-link per cell (`#PT-D5-03`)
- View the score summary by domain
- See the Pre-filter (UNICEF + ESSA Tier 1/2) and the 8 binary Disqualifiers
- Review the literature anchors and structured-pedagogy diagnostic instruments

## Source files

- `index.html` — single-file static browser (Tailwind CDN, vanilla JS)
- `rubric_v7_4.json` — extracted from `Logging_Rubrica_LXP_ElSalvador_v7_4_COMPLETE.xlsx` via `scripts/extract_rubric_to_json.py`

## Deploy

This site is designed for **GitHub Pages**:

1. Create repo `lxp-elsalvador-rubric` in your GitHub account
2. Push these files to `main` branch
3. Settings → Pages → Source: `main` / root
4. Done. URL: `https://<username>.github.io/lxp-elsalvador-rubric/`

To update the rubric data: re-run `extract_rubric_to_json.py` against the latest XLSX, copy the resulting `rubric_v7_4.json` into this repo, commit, push.

## Reports

The full Assessment PDFs (Spanish + English, ~50 pages each) and the Evidence Detail PDFs (~80 pages each with verbatim transcripts and screenshots) are in the source repository alongside the rubric XLSX.

## License & attribution

Banco Mundial · Equipo Educación LAC · 2026.

This rubric synthesizes 5 primary frameworks (GEEAP 2023+2024, Rosenshine 2012, ESSA Tier 1-4 + WB EdTech series 2023-2024, BEA shared task ACL 2024+2025, Khan/IXL/ALEKS adaptive-learning literature) and 18 secondary sources. The full source list is in section 1.1 of the Assessment PDF.

Independent reuse of the rubric for procurement evaluation in other LAC contexts is encouraged — please cite the World Bank LAC Education team and the rubric version (v7.4, May 2026).
