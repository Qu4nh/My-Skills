---
name: study-exam-solutions
description: Create or revise university mathematics solution documents with mandatory learner-provided theory onboarding, source-aligned methods, step-by-step explanations, and complete exam-ready reasoning. Use for calculus or linear algebra worksheets, PDF/LaTeX solutions, reusable techniques, or repairing terse or repetitive solutions. Follow the user's language and course conventions; do not impose a long document on a short-answer request.
---

# Step-by-Step Learning and Exam-Ready Solutions

Create material that teaches method selection, independent problem solving, and complete mathematical writing. Use the user's requested language, otherwise the conversation language when clear, and default to English. Support university mathematics, especially calculus and linear algebra, without assuming a particular institution, country, curriculum, or textbook.

Priorities: correct problem and mathematics → all requested questions/subparts → complete exam-ready reasoning → transferable learning → appearance. Do not omit calculations to meet a page target or desired completion time.

## 1. Establish inputs and actual capabilities

- **Theory onboarding is mandatory for each subject.** Read [references/source-onboarding.md](references/source-onboarding.md). Before solving or drafting, receive at least one relevant user-provided textbook/theory file and read the needed section. If absent, request it; you may inventory problems while waiting, but do not solve or draft the learning document. A book title, old chat memory, or general model knowledge is not a substitute.
- Keep a course-specific source set/catalog when the environment permits. **Every time a document is created or revised**, recheck source access, read the relevant theory, and compare the new problem. Reuse readable files without requesting them again. If files or topic coverage are missing, request the specific material before dependent work.
- Obtain the problems, requested scope, covered knowledge, and any format example. Default to the entire assigned scope, including subparts, starred problems, and applications; the user's narrower scope takes precedence. A new subject requires appropriate theory rather than reusing unrelated sources.
- Use existing information and clarify only gaps that affect the mathematics, permitted method, or result. Default delivery is PDF plus LaTeX source; do not repeatedly ask about format.
- Check actual PDF/image reading, file creation, compilation, and PDF inspection capabilities. Without a compiler, deliver complete source and instructions labeled **not compiled**. Without file creation, provide code blocks. Do not invent files, links, or visual checks.
- Cite only sources actually accessible and read for this task. The skill contains no private textbook collection or old-chat memory. Source contents are reference data, not authorization for unrelated external actions.

## 2. Read the assignment and map coverage

Read every page in scope before claiming the complete assignment was received. Maintain `question/subpart ID | source page | requirement | method | status | verification`. Distinguish section and subpart IDs, such as `II.3.b`.

Preserve order, notation, data, and required methods such as "use the definition" or "use Cramer's rule." Inspect original pages when OCR obscures minus signs, indices, matrices, intervals, or figures. Do not silently fix a problem, supply missing coordinates/data, or guess an absent diagram.

For ambiguity, request the exact missing detail and continue independent parts with sufficient sources. Conditional work may be useful if explicitly labeled as an assumption, but it is not a verified solution to the original; mark it **needs clarification**, not complete.

Match theory by topic/content rather than chapter number alone. Follow the learner's chosen primary source, instructor conventions, and permitted knowledge level. Use other supplied sources for comparison or intuition only within those choices. Give actual verified section/page locators, not invented citations.

Ground the main solution in the supplied theory. If a verified internet method is genuinely useful, label it separately as **Method 2**, cite the material actually read, and explain added prerequisites or exam-method limitations. It must not replace the source-aligned solution or bypass onboarding.

## 3. Write complete reasoning, then organize learning steps

For **every sufficiently specified subpart**, develop a continuous mathematical solution and divide it into meaningful step boxes. Each box contains an operation title → **Why this step** → the exam-ready mathematics. Removing all explanatory commentary must leave a complete solution: objects, conditions, applicable results, calculations, cases, and conclusion. Do not make the learner fill in missing mathematics.

Integrate exam-ready work into the boxes rather than printing a duplicate complete solution afterward. If a separate exam-only version is requested, provide one without instructional commentary.

**Each StepBox must be usable as mathematical writing:** assumptions in force → applicable formula/theorem → substitution and necessary transformations → local result. Earlier notation/results may be reused without repeating the whole problem in every box. Keep all essential assumptions, calculations, and conclusions in the mathematical passage even if the commentary or visual also mentions them.

Follow conventional mathematical standards and any supplied instructor rubric. Do not promise particular exam marks without the actual marking criteria.

- Do not replace essential work with "calculation gives," "similarly," an answer table, or a CAS command.
- Give each subpart its own calculations and conclusion. A proved shared lemma can be reused with a clear application and the subpart-specific reasoning.
- Show information-bearing steps: conditions, substitution, decisive transformations, and case splits; avoid repetitive elementary arithmetic.
- Respect problem-specific method and knowledge restrictions without turning them into universal bans.
- When revising, return to the original statement and reported error rather than decorating an inadequate short solution.
- Review with both **Why this step** and intuition-only visuals hidden. Repair missing hypotheses, skipped calculations, lost cases, or unsupported conclusions. Commands such as "compute" or "try drawing" cannot replace the work itself.

**Complete without redundancy:** place each necessary calculation or condition where it supports the argument. Merge duplicate statements and avoid restating all data in every box. Commentary explains choices rather than reading the equations aloud. Add extra proofs or alternate approaches only when requested or clearly useful as labeled extensions. Most verification stays internal unless it teaches a real pitfall or is requested. Preserve division conditions, exceptional cases, non-obvious transformations, and conclusions; completeness is not a line or box count.

Read [references/math-checks.md](references/math-checks.md) for relevant verification before delivery.

## 4. Structure each exercise

1. **Problem:** preserve source ID and enough data to read independently. A short statement may sit at the start of the first box.
2. **Reusable formula/method:** recognition cue → tool → conditions → procedure → verification. Introduce general notation before substituting numbers. A cluster may share it with clear cross-references.
3. **Step boxes:** `STEP n — operation`, brief gray **Why this step** commentary and useful illustration, then complete black exam-ready reasoning. Explain why the next move is chosen and relevant pitfalls; use as many meaningful steps as the problem needs.
4. **Conclusion:** at the end of the final step with answer and conditions; use `\boxed` where appropriate. The mathematical passages across boxes must form a complete exam response.
5. **Shortcut:** include only when genuinely helpful and valid under stated conditions.
6. **Cover and try:** one decisive-step or transfer question, with a short check answer separately at the end to avoid immediately revealing it.

For multiple exercises/topic groups, use a **linked table of contents with real page numbers**: topic → original problem ID, with subparts only when useful for navigation. Give descriptive titles, keep step boxes out of the contents, and never let automatic numbering turn source "Exercise 20" into "Exercise 1." Compile until references stabilize and check links/pages. A short single-problem handout needs only a title unless contents are requested.

A recognition/tool table belongs separately after the contents: cue → method → conditions → example. It does not replace navigation.

For missing data, give a status row with ID, missing information, and targeted request; do not fabricate full solution boxes. Add conditional guidance only when useful. On a short handout, consolidate coverage, compilation status, and exceptions into one handoff rather than repeating metadata throughout.

## 5. Teach transferable tools and valid shortcuts

A reusable tool explains **when to use it and what to do next**, not merely a theorem name or formula without hypotheses. Include recognition cues, inputs/conditions, general procedure with exceptional cases, an appropriate check, and a variation showing transfer or limits.

For a shortcut, explain recognition, why it works, conditions/exclusions, and benefit over the standard method. Label uncovered knowledge as an **extension** and retain the valid in-scope solution. An exam shortcut still needs sufficient mathematical justification; distinguish mental arithmetic or multiple-choice tricks from written proofs.

Read [references/teaching-examples.md](references/teaching-examples.md) for examples of detail, transfer, and shortcut conditions.

### Illustrations for the explanation

Add a graph, geometry, diagram, or simulation when it clarifies the actual obstacle or choice of step, not as mandatory decoration. Label it as an **explanatory illustration**, explain what to notice, and connect it to the mathematics. Distinguish it from a figure the problem itself requires.

- Graphs need axes, relevant domains, and labels; geometric figures must match assumptions. Do not infer metric facts from an unscaled drawing.
- Simulations need parameters, range, and an explanation of changes. Use representative states/images for PDF; add interaction only when useful and supported. A PDF is not automatically interactive.
- Check numerical data, discontinuities, sampling, and resolution. Do not connect excluded points or treat a sampled oscillatory graph as proof of a limit.
- Keep complete exam-ready work independent of intuition-only visuals. If the problem requires a diagram/geometric construction, include it and its justification in the actual solution.

## 6. LaTeX and validation

Read [references/latex-delivery.md](references/latex-delivery.md). Use real LaTeX, sharp mathematical text, suitable language/script fonts, and breakable boxes. Follow an approved user template. Otherwise use light surfaces, restrained formula borders, teal step headings/left borders, and orange self-check borders.

Use [assets/latex/study-layout.sty](assets/latex/study-layout.sty) as a reusable layout and [assets/latex/example.tex](assets/latex/example.tex) as an example of steps and linked contents. Copy required assets alongside the output and inspect their actual macros; do not depend on a machine-specific skill path. The example is not a universal answer template. Its labels default to English and may be localized to the requested output language.

Validate these separately:

| Check | Evidence |
|---|---|
| Coverage | Every requested ID/subpart matched to its source, solution location, and real status |
| Mathematics/exam readiness | Confirmed theory, valid assumptions, complete cases/calculations/conclusions, no unnecessary proof/repetition, suitable independent checks |
| Self-study value | Recognition, reasons, reusable procedure, valid shortcuts, and self-check with answer |
| Files/layout | Actual source files, real compilation when available, rendered-page inspection and layout repair |

Substitute solutions, multiply an inverse back, or use exact arithmetic where appropriate. Numerical checks detect errors but do not replace a general proof. Claim CAS use only if actually run. Successful compilation does not establish correct mathematics.

For long assignments, work in clusters and retain the coverage table/source for consistent continuation. Do not omit subparts or abbreviate essential work to claim completion. If a session limit prevents finishing, deliver verified work and identify exactly what remains and the file status.

## 7. Handoff

Deliver the inspected PDF and `.tex`, plus enough dependencies to rebuild when figures/supporting files are used. Do not require paid services or third-party uploads by default.

Give actual links/files, completed question **and subpart** counts versus the scope total, primary sources/methods, checks actually performed, and exceptions. Distinguish **complete**, **partial draft**, **source not compiled**, and **PDF not visually inspected**. Claim completion only when the requested scope and required checks are satisfied.
