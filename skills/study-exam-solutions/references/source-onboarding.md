# Mandatory theory onboarding and source reuse

## First use for each subject

1. Inspect attachments and the saved source set for this subject. Require at least one **user-provided textbook/theory file** with readable relevant content. A problem sheet's short preamble is not automatically a theory source unless it actually provides the needed course theory and is identified as such.
2. If missing, request the course's textbook/theory file and subject if unknown. Explain that it is required and will be reused for later worksheets. Do not write solutions or a learning PDF before this gate is met. You may read and inventory the problems while waiting.
3. Inspect actual content: table of contents, relevant topics, readability, terminology, and taught methods. Record only verified portions, not a claim to have read an entire book after one chapter. Inspect original scanned pages or request readable copies when needed.
4. Establish the preferred source and any chapter/knowledge limit. Follow the user's priority when sources differ; clarify only conflicts that affect the solution. Do not replace chosen theory files with web sources.

## Preserve sources for later work

When supported and permitted, keep files or durable accessible paths in the user's workspace by subject, for example `study-sources/calculus-1/`. Preserve names or an explicit mapping and do not overwrite unrelated files. A `sources.json` catalog can record subject, file, role, verified topics/sections, and access status; use a hash when useful for detecting changed versions. A summary is an index, not a substitute for the real file.

```json
{
  "course": "calculus-1",
  "theory_sources": [
    {
      "file": "files/course-textbook.pdf",
      "role": "primary",
      "verified_sections": ["Actual chapter or topic read"],
      "status": "readable"
    }
  ],
  "knowledge_scope": "Scope supplied by the learner or verified in the material"
}
```

In chat-only environments, use files actually accessible in the current chat/project and record confirmed sources. Do not promise memory or access across chats when unavailable. If a new session lacks the files, request reattachment; an old list of book titles is insufficient.

Do not include private textbooks in a reusable skill, distribution bundle, or handoff unless the user requests it. Course sources belong to the task/workspace, not the global skill installation.

## Every document creation or revision

- Verify subject/catalog and actual file readability. If missing, corrupt, or lacking the needed section, request the specific addition and stop dependent work rather than silently using memory/outside sources.
- Read the new problem and corresponding theory, matching by topic rather than chapter number alone. Map problem type → source definition/theorem/method.
- Preserve confirmed notation, reasoning style, level, and permitted methods. When a problem explicitly requires a different approach, identify the difference and satisfy the task. Request missing theory where needed rather than substituting an advanced trick.
- Identify ambiguity or conflict instead of silently repairing the statement to match theory. Continue independent problems with sufficient sources.
- Cite actual file/chapter/section/page briefly at the cluster or source-list level; repeat at an exercise only when helpful. Do not invent pages or cite the same theorem on every line.
- Source alignment does not mean copying textbook solutions or skipping mathematical verification. Maintain full subpart coverage and exam-ready reasoning.
- A useful external method must be a separate, verified, cited Method 2 with added prerequisites and exam limitations. It cannot replace onboarding or the main in-scope solution.

| Source status | Action |
|---|---|
| No suitable theory | Request the file; do not draft solutions |
| Confirmed and readable | Reuse it and read the section for the new problem |
| Catalog exists but file/access is missing | Restore access; do not treat the catalog as reading evidence |
| New subject or missing topic | Obtain the appropriate theory before affected work |
