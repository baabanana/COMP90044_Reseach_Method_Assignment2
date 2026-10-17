# COMP90044 Activity 1 — fast Overleaf template

This project is intentionally small and uses **pdfLaTeX + BibTeX**, which is a
good fit for Overleaf's free compile limits. The default reference style is
IEEE because the assignment sheet explicitly requires IEEE formatting.

## Use on Overleaf

1. Upload `COMP90044_Activity1_Overleaf.zip` as a new project, or upload
   `main.tex` and `references.bib` together.
2. In **Menu → Settings → Compiler**, select **pdfLaTeX**.
3. Edit the four fields near the top of `main.tex`.
4. Replace the italic guidance with your own 300–500 word introduction.
5. Add about 16 real peer-reviewed conference or journal papers to
   `references.bib`. Keep DOI fields where available.
6. Adjust the proposed structure so it matches your topic.
7. Click **Recompile**. Overleaf automatically runs BibTeX when needed.

The line `\nocite{*}` makes every valid `.bib` entry appear in the reference
list, even if it is not cited in the introduction. This is useful for Activity
1's indicative list of approximately 16 references.

## Citation commands

- `\citep{zhu2017bestconfig}` produces a parenthetical numeric citation in the
  required IEEE setup, such as `[1]`.
- `\citet{zhu2017bestconfig}` can be used when the authors are part of the
  sentence.
- Multiple sources: `\citep{key1,key2,key3}`.

The Zhu et al. paper is already included as a complete BibTeX example. Under
the required IEEE style it is rendered as a numbered reference rather than the
APA-like author–year entry shown in the request. Do not switch to APA unless
the teaching team confirms that it is acceptable.

## BibTeX templates

Journal paper:

```bibtex
@article{surname2026shorttitle,
  author  = {Family, Given and Family, Given},
  title   = {Full Article Title},
  journal = {Journal Name},
  year    = {2026},
  volume  = {00},
  number  = {0},
  pages   = {1--20},
  doi     = {10.xxxx/xxxxx},
  url     = {https://doi.org/10.xxxx/xxxxx}
}
```

Conference paper:

```bibtex
@inproceedings{surname2026shorttitle,
  author    = {Family, Given and Family, Given},
  title     = {Full Conference Paper Title},
  booktitle = {Proceedings of the Full Conference Name},
  year      = {2026},
  pages     = {1--10},
  publisher = {Publisher},
  doi       = {10.xxxx/xxxxx},
  url       = {https://doi.org/10.xxxx/xxxxx}
}
```

## Keeping compilation fast

- Keep pdfLaTeX; do not change to XeLaTeX or LuaLaTeX.
- Keep BibTeX; do not replace it with `biblatex`/Biber just for APA formatting.
- Compress large figures before upload. Activity 1 does not require figures.
- Use Overleaf's **Word Count** menu rather than adding a word-count package.
- If references look stale, use **Recompile from scratch** once; ordinary edits
  should use the normal Recompile button.

## Checklist before submission

- Introduction is 300–500 words and describes the nature of the problem.
- Claims in the problem description are supported by citations.
- Approximately 16 suitable references are listed.
- References are peer-reviewed conference or journal papers and include DOI
  links when available.
- The proposed structure explains how the final review will be organised.
- Placeholder guidance and the demonstration sentence have been removed.
