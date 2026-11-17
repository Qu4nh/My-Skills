# Long-session state and evidence

## Observed learning states

Track per course, topic, and technique rather than assigning one level to an entire chapter or all mathematics:

| State | Meaningful evidence |
|---|---|
| Not yet studied | No explanation/practice in the accessible record |
| Explained | Tutor explanation or a viewed worked example |
| Performed with help | Actual learner work after specified hints |
| Performed independently | Actual self-produced work and adequate reasoning, with ID, conditions, and scope |
| Needs review | Important unresolved error or unstable recall; retain correct parts of earlier work |

When a checkpoint merely claims mastery without evidence, preserve it as **self-reported, unverified**. Neither erase it nor treat it as verified. One multiplication does not establish Gaussian-elimination mastery; a routine derivative does not establish limit proofs, and a probability calculation does not establish statistical inference. Do not invent mastery percentages.

Keep a separate source map and progress scope for each course. A switch from linear algebra to calculus, probability, or another subject requires appropriate theory onboarding. Preserve the previous course's progress; do not transfer its confirmed level to an untested subject. Explicitly link any genuinely applicable prerequisite evidence without counting it as a passed check of the new technique.

A/B/C classifies exercise novelty, not competence. A new technique shown in a worked solution remains only explained; skipping is not completion.

## Skill map and confirmed levels

Selectively adapted from [Jane Street's socratic-tutor](https://github.com/janestreet/agent_skills/blob/master/socratic-tutor/SKILL.md); the attribution and MIT notice are included at the end of this reference. Derive techniques from actual problems and theory, not a fixed item count.

| Level | Demonstrated ability |
|---|---|
| ? | Insufficient evidence; not automatically 0 |
| 0 | Diagnostic evidence of not yet recognizing the concept |
| 1 | Recognizes/has heard of it, but cannot yet follow the method |
| 2 | Follows a solution and explains its operations |
| 3 | Performs with hints |
| 4 | Solves and reasons independently within the recorded scope |
| 5 | Explains clearly to someone else and handles an edge case/difficult variant |

Confirming level 4 or 5 requires **at least two independent checks**, including unprompted recall/application after intervening material or in a later session. Repeating a just-provided answer is not independent. Level 5 also needs explanation and edge-case evidence. Levels 0–3 describe directly observed behavior without unnecessary repetition just to meet a count. Preserve a single independent performance even when level 4 is not yet confirmed.

Keep **performance events**, **confirmed level**, and **review flags** separate. A failed review warrants a targeted adjustment based on the error/help needed, not erasing all progress or demoting a chapter. Preserve old checkpoint evidence with an unconfirmed level rather than converting labels mechanically.

Evidence identifies the actual problem/step, checked result, reasoning seen, help given, and when the later recall check occurred. "I know it" or "I did many problems" does not newly confirm level 4/5. Label handed-off history as such; do not claim to have directly observed it. For current confirmation, inspect concrete work or set an appropriate task and verify it. Partial correctness or vague reasoning is not a fully passed check.

At a study session's start, show a compact map: `topic/technique | current level | target | evidence/limits | next`. Report a short update after each level change; show the relevant full table on request or at cluster transitions. Do not turn summed ordinal levels into an overall percentage.

Queue reviews with technique, reason, and a learning-sequence trigger such as "after another technique" or "next session." At that point, inspect the queue and review or explicitly defer. Never fabricate completed review history.

The default practice target is level 4 in the agreed scope, or level 5 when deeper mastery is requested. The learner may change the goal. **Session paused**, **material covered**, and **completion verified** are different outcomes.

For a mixed assessment, map every technique to an actual question/subpart and include a connection or method-selection task. Keep Method 2 outside scope unless explicitly included. One problem may assess multiple techniques if each has identifiable evidence. Do not confirm completion with incomplete assessment coverage or an unmet target. Report the final map, achieved scope, and weak areas; the learner can stop and return later.

## Transfer checkpoint

Provide copyable Markdown containing only supported facts. Use "no evidence yet" or "not recorded" as appropriate; do not infer state from examples in this skill.

```markdown
# University Mathematics Checkpoint
- Updated: [known date or learning milestone]
- Provenance: [observed here / learner handoff / mixed]
- Language and learning preferences: [explicitly requested or supported by feedback]
- Learner profile: [revision and actual accessible content/location; include a compact snapshot when transferring]
- Profile snapshot: [goal, relevant teaching/format preferences, time/exam constraints, unknowns; distinguish self-report from observed ability]
- Current-turn overrides: [temporary instruction and scope, or none]
- Course/subject: [actual course, current topic, and prerequisites]
- Materials: [actual filenames, roles, verified sections/pages]; recheck access in a new chat.
- Theory onboarding: [topics ready / missing file / missing section / access needs restoration].
- Method 1: [primary file, verified locator, definitions/theorems/procedure].
- Method 2: [actual URL read, benefit, added prerequisites; or not used].
- Location: [chapter/section/question/subpart and verified source locator]
- Current objective: [concept or step]
- Agreed scope and target: [techniques, level 4/5 or other learner goal]
- Awaiting learner: [exact task/result, or none]
- Mode: [guided practice / full solution for specified scope / assessment]

| Course/topic/technique | Observed state | Confirmed level ?/0–5 | Evidence and limits |
|---|---|---|---|
| [technique] | [state] | [supported level] | [ID, learner work, help, independent checks, cases handled] |

- Misconceptions: [specific issue and repaired/unresolved status]
- Review queue: [technique, reason, after another topic/next session; or none set]
- Mixed assessment: [actual scope/results, or not done]
- Assessment coverage: [technique → actual question/subpart; connection task; unchecked parts]
- Scope outcome: [paused / covered but unverified / completion verified with evidence]
- Exercises scanned: [range actually read and missing parts]
- Gaps/skips: [ID, unstudied cases, reason]
- Next action: [one concrete step and missing dependency if any]
- Unverified: [source, history, or work still needing confirmation]
```

Record the pending question, not a hidden answer to the same assignment. A learner-visible checkpoint must not expose a result they have not yet produced.

## Update cadence

- Update meaningful events, not every utterance, and preserve source IDs.
- At a cluster/section transition, give a short factual marker, for example: "You formed the minor independently; cofactor signs still need review. Next is transposing the cofactor matrix." Use it only when those facts are true.
- At the end or transfer, supply the checkpoint rather than merely saying it was saved. If writing a file, name its actual path; another agent does not automatically receive it.
- Transfer enough of the learner profile to reproduce the teaching choices, not just a filename. Keep personal records outside the shared skill/repository, preserve uncertainty/provenance, and do not turn preferences into competence levels. Current explicit corrections update the profile without resetting unrelated progress.
- On resumption, recheck theory access/scope and restore the source gate before teaching or grading. Ask only for missing files/sections, not the whole history. Keep Method 1 evidence separate from Method 2 extensions.

## Third-party attribution and license

This skill adapts selected tutoring and progress-assessment ideas from Jane Street's
`socratic-tutor`: https://github.com/janestreet/agent_skills/blob/master/socratic-tutor/SKILL.md

The local adaptation preserves the learner's requirements for ELI5 explanations,
illustrations, mandatory course-material onboarding and separate internet methods.
It does not reproduce the upstream skill unchanged. The upstream license follows.

The MIT License

Copyright (c) 2026 Jane Street Group, LLC <opensource-contacts@janestreet.com>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
