# Flexible chat interaction and mathematical media

## Open format, concrete purpose

Choose or combine any response format that fits the learner's goal, evidence, current mode, and actual host capabilities. Examples include multiple-choice or multiple-select quizzes, fill-in fields, matching, ordering, error spotting, open reasoning, annotated work, static/dynamic graphs, retrieved or original images, geometry, manipulatives, simulations, audio, and other supported media. This list is illustrative, not a whitelist. There is no skill-imposed fixed item count, number of visuals, response length, or requirement to show the same headings in every turn.

Honor the requested format and scope when useful and supported. Keep onboarding/source fidelity, mathematical accuracy, the agreed learner answer boundary, and evidence standards intact across formats. A larger quiz or comparison is allowed; avoid unnecessary output that adds no learning value. Ask about format only when a meaningful ambiguity remains, not before every response.

## Check what the host can actually do

Use the available tool/surface documentation or a successful tool result to establish rendering and interaction capabilities. Do not assume a specific product, plan, app name, markdown support, or a previous agent's capability guarantees a feature here.

- If a suitable native quiz, form, plotting, canvas, image, or interactive artifact tool is available, use it when it serves the requested task. Follow that tool's execution/permission contract.
- If native interaction is unavailable, a text quiz can accept letters, a blank activity can accept numbered responses, and a static visual can replace unsupported interactivity. Explain the limitation briefly and supply the actual usable activity rather than repeatedly asking the learner to install something.
- Writing `[ ]`, an HTML input, a "button" label, or a code block does not create a clickable/gradable control in ordinary chat. Do not claim auto-submission, stored answers, grading callbacks, sliders, or a rendered chart without actual support.
- Do not announce tool absence without checking the capabilities exposed to the agent. Equally, do not expose the learner to implementation steps when a working in-chat result can be produced directly.

## Quizzes and fill-in activities

Use plausible alternatives based on actual misconceptions and confirm the question has the intended valid answer set. Identify single-choice versus multiple-select, units, precision/tolerance, and any assumptions affecting uniqueness. Avoid distractors that are accidentally equivalent to the intended answer. Shuffle or vary answer positions when useful; there is no required option count.

For fill-ins, label the blanks and indicate what type of response belongs there. Allow equivalent mathematical expressions when the exercise tests meaning rather than an exact spelling. For matching/ordering, specify how to submit the mapping or sequence. A learner-requested batch can contain multiple tasks and blanks; do not force it into a one-item loop.

For an unanswered learner activity, end at a clear answer checkpoint and keep the answer key out of prose, captions, code, visible metadata, or collapsible blocks delivered to the learner. In a native interactive tool, place correct answers in its actual non-visible grading configuration only if that visibility is documented; if uncertain, do not assume that a tool argument is hidden from the learner. Native automatic feedback is appropriate only if supported and consistent with the requested timing. When a worked example or explicit key is requested, provide it in that mode rather than pretending to assess unaided performance.

After the learner responds, verify the mathematics independently of a widget score. Recognize correct parts, interpret the chosen distractor or blank, and explain the actual misconception. An option chosen correctly is evidence of recognition within that item; a partially supplied derivation is scaffolded performance. Neither alone proves independent construction, transfer, or delayed recall. Record help, format, attempts, and limitations with the learning evidence.

## Show graphs and interactive mathematics in the chat

When a graph helps or is requested, produce and display a real plot through available plotting/rendering/artifact tools instead of merely describing a future graph or supplying code to run. Use any suitable renderer; do not impose one plotting library or file type. Prefer native inline output when available, otherwise embed a verified generated artifact in a way the host supports. If the host cannot display it, provide an accessible alternative and label it accurately.

For a static or interactive graph, check mathematical content: function/domain, axes and scale, units, labels/legend, endpoints, holes, asymptotes, discontinuities, and sampling behavior. Do not connect through undefined points or present a sampled plot as a proof. For a slider or dynamic diagram, state the parameter, valid range, and what changes; verify a few meaningful states, including relevant boundaries. Keep controls usable and provide a static/text equivalent when interaction is unavailable or inappropriate for the learner's format needs.

Inspect the produced visual before claiming it is correct and displayed. Captions should point to what the learner should notice. An exploratory graph must not expose an answer deliberately reserved for the learner's current task; choose different data, limit annotation, or change the activity so the plotted information is intentionally what is being assessed.

## Retrieve, reuse, or create images

Choose the best source for the concept: an accessible course figure, a retrieved explanatory image with a verified source, an original diagram, or a mathematically computed graphic. Use available image search/browser tools when retrieval is requested or useful; actually view candidate images and check their mathematical labels, relevance, and provenance. Do not invent an image URL or claim to have found/viewed one from a search snippet.

Display a retrieved image inline when the host permits and cite its real source near it. A source link remains useful but does not by itself meet a request to see the image in the chat. Respect host embedding/download restrictions and preserve required attribution or reuse conditions. If embedding or retrieval is unavailable, say so briefly and supply a labeled original representation or other usable fallback without calling it a retrieved image.

A visual does not become Method 2 merely because it came from the web. A sourced picture illustrating the same onboarded course method can support Method 1 with attribution; a genuinely different outside technique belongs in Method 2 with its prerequisites and exam limitations. Learner-provided source theory is still required.

For exact mathematical plots or geometric constructions, use a method that preserves the equations, data, and labels and verify the output. Generative illustration can help conceptual imagery when available, but do not assume generated text, axes, measurements, or mathematical geometry are exact; check or replace them. No one image-production technique is mandated.

## Transfer and persistence

Remember content and state, not an unsupported promise that a widget will survive another chat. In a profile/checkpoint, record the preferred formats, confirmed host limitations, relevant accessible artifacts, activity IDs/items, already submitted work, feedback shown, and remaining answer checkpoint. Keep unanswered keys out of learner-visible transfers. A native widget does not automatically carry across agents or platforms; reconstruct the activity from safe, accessible task data when needed.

Current requests can override a stored preference: someone who normally likes prose may request a graph or a multi-item quiz today. Do not lock them into a permanent format category, and do not reset mathematical progress when switching representation.
