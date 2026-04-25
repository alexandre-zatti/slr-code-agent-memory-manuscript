# Codex Instructions - SLR Manuscript

This directory contains the LaTeX manuscript. The parent
`revisao-sistematica/AGENTS.md` remains authoritative for project-level rules.

## Before Editing

- Read `PLAYBOOK.md` before drafting or changing prose.
- Check `../PROGRESS.md` for current manuscript status.
- Verify citation keys in `references/included-studies.bib` before writing
  `\citep{}`, `\citet{}`, or `\cite{}`.
- Use one sentence per line in `.tex`.
- Preserve the manuscript's English venue style: JSERD primary, EMSE secondary,
  author-year `natbib`.

## Build And Checks

From this directory:

```bash
latexmk -pdf main.tex
```

From `revisao-sistematica/`:

```bash
bash manuscript/scripts/academic-gate full
bash manuscript/scripts/academic-gate visual
```

Run rendered visual QA whenever figures or tables changed. The normal
`academic-gate tier1` path runs deterministic visual checks without PNG
rendering; `academic-gate visual` generates the PNGs for manual inspection.
Zero CRITICAL and zero MAJOR issues are required before considering a section
done.

## Prose Rules

- Use the denominator terms from `../AGENTS.md`: included studies,
  architecture studies, controlled-comparison studies, and contextual studies.
- Do not use "primary studies" in manuscript prose.
- Prefer concrete counts and conditions over broad claims.
- Verify Tier A/B/C claims against JSON/TSV, digests, or PDFs before asserting
  them.
- Keep de-AI cleanup proactive: avoid formulaic transitions, banned buzzwords,
  em-dashes, and uniform paragraph rhythms.

## Generated Files

Do not commit LaTeX build artifacts unless explicitly requested. The public
mirror is published through `../scripts/publish-manuscript.sh`, not by manual
copying.
