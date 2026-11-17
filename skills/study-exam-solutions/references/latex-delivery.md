# LaTeX, layout, and delivery

## Source and design

Default to A4 unless the user/course specifies another paper size, 11–12 pt type, margins near 2 cm, readable mathematics, and contents/bookmarks/page numbers for longer documents. Use Unicode source and an available XeLaTeX/LuaLaTeX setup with fonts covering the requested output language. For scripts needing shaping, directionality, or language-specific typography, configure and verify appropriate language/font support rather than assuming an English template renders them. Use pdfLaTeX only with a verified encoding/language setup. Do not rasterize ordinary text/equations into screenshots.

Use `amsmath`, `amssymb`, `geometry`, `graphicx`, and `hyperref`; use `tcolorbox` with `breakable` for long boxes. Add other packages only when needed. Define reusable environments for formulas, learning steps, shortcuts, and self-checks.

- Formulas: thin restrained border and white/very light background.
- Learning steps: pale teal heading band, dark teal left border; commentary visibly distinct from calculations.
- Exam-ready work: black mathematical passages in each step box below gray **Why this step**. Removing commentary leaves a complete answer. Add a separate full solution only if requested.
- Explanatory illustration: labeled graph/geometry/diagram or representative simulation states, with captions, before the mathematical passage. Use sharp/vector graphics and avoid floats drifting into another step. Keep graded calculations and arguments in the mathematical passage. A figure required by the problem is part of the actual answer.
- Shortcuts: separate label and visible conditions.
- Self-checks: orange border with short answers at the end.

Keep headings with their opening lines and allow sensible box breaks. Split long matrix/elimination chains rather than shrinking them into unreadability. Use `aligned`, `split`, or `multline` for long equations. Do not put a multipage solution in an unbreakable box.

Figures must preserve problem data/labels. Prefer original or verified reconstructions and label approximate graph readings. Do not invent a figure to fill a missing statement.

## Bundled layout and linked contents

Copy `assets/latex/study-layout.sty` and `example.tex` into the output source directory and replace example content with the actual assignment. `FormulaBox`, `StepBox`, `Why`, `SelfCheckBox`, and `QuickTipBox` provide consistent reusable elements.

The template's default labels are English. Localize them for the requested language through the `Study...Name` commands with `\renewcommand`; retain mathematical/source IDs. Font choice must be checked for the output script. A style default is not a requirement to translate a learner's source notation.

`ExerciseGroup` makes topic sections; `Exercise` takes an original ID and description; `ExercisePart` adds subparts. Use unique labels across chapters/files. `StudyContents` provides linked contents, pages, and bookmarks; do not list StepBoxes. Default `tocdepth=2` shows groups/problems; use 3 when actual long subparts need navigation. `BackToContents` returns to the contents.

Contents must match the real document, preserve source IDs, and have compiled page numbers rather than manually typed values or unresolved question marks. Distinguish repeated exercise numbers by group/labels. Recompile until references/contents stabilize and test at least each group's link and the last exercise.

The example uses Exercise 20 on a derivative at a joining point and Exercise 7 on a parameter system. These demonstrate navigation and complete reasoning, not a required curriculum. Do not invent subparts to show hierarchy. The style selects Times New Roman when available and otherwise TeX Gyre Termes; choose another suitable font for languages/scripts it does not cover. Colors never justify omitting calculations or making text too small.

## Compilation

Check which engine is available. In the source directory, for example:

```sh
xelatex -interaction=nonstopmode -halt-on-error main.tex
xelatex -interaction=nonstopmode -halt-on-error main.tex
```

Use `latexmk -xelatex main.tex` if already available. Multiple passes update references/contents; still inspect logs for unresolved references, missing fonts/images/glyphs, and significant overflow. Do not enable unnecessary shell escape or external code.

Repair source and recompile after errors. A successful command validates typesetting, not mathematics.

Before compilation or a source-only handoff, check balanced math delimiters/environments and keep math-only commands such as `\boxed` inside math mode. "Not compiled" reports a capability limitation; it is not a reason to skip syntax review.

## PDF inspection

Render every page at useful resolution when supported. Inspect the first/last pages, group boundaries, tables, figures, wide matrices, and page-splitting boxes. If inspecting a subset, report that actual scope rather than claiming a full review.

Check characters in the requested language, scripts/directionality where relevant, indices/exponents, symbols, image sharpness, clipped equations, unusual blank areas, stranded headings, and independent readability of exam-ready passages. Reinspect affected pages after repairs.

Check axes, domains, labels, captions, and simulated states in explanatory visuals. Keep the distinction between intuition and formal work clear. Do not delete calculations or shrink a solution to make space for a visual.

## Rebuilding and handoff

Provide `.tex` and required assets with relative paths. State engine, any special font/packages, and minimal compilation command. Do not bundle full private textbooks, chat history, caches, or machine-specific dependencies.

For multiple assets, make a source ZIP and try a clean-directory rebuild when tools permit. Verify delivered files and links. Checking a file list is not a tested rebuild.

Without an engine, deliver complete source/assets labeled **not compiled**, plus commands. Use the learner's chosen editor/service if requested; do not upload their sources to external services automatically. Without PDF viewing, report **not visually inspected**. In chat-only environments provide UTF-8 source code and instructions for saving `main.tex`.
