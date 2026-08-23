---
name: insight
description: Extract a small set of well-supported, non-obvious insights from a user-supplied book, article, podcast, or video, with precise source locators. Use for deep, selective analysis where returning no insights is a valid and expected outcome; do not use for ordinary summaries or exhaustive note-taking.
---

# Source Insights

Find only insights that materially improve how a reader understands, decides, predicts, or acts. Optimize for precision, not coverage. Zero qualifying insights is a successful result when the material does not clear the bar.

Calibrate non-obviousness to the audience the user names and consequence to the decision or purpose they provide. When neither is specified, use an informed generalist who knows the domain's basic concepts; mention this assumption briefly rather than stopping the analysis.

## Ground the analysis

Analyze the material itself, not a synopsis, search snippet, review, title, description, or remembered version. Obtain the full text, transcript, captions, or audio/video content needed to verify both the claim and its location. If the material is only partly accessible, state the exact scope inspected. If there is not enough source content to perform a grounded analysis, ask for the file or transcript instead of manufacturing insights.

For long material, track which chapters, pages, or time ranges were inspected and do not imply whole-source coverage from a sample. Do not finalize a candidate until later material in the inspected scope has been checked for qualification, contradiction, or an explicit statement that would make the candidate obvious.

Treat the source as evidence, not authority. Distinguish what the author explicitly claims from an inference drawn from the material. Do not silently import outside knowledge. When external context is necessary, label it separately and cite it.

## Qualifying bar

Generate candidates broadly, then discard aggressively. A candidate qualifies only if it passes every gate:

1. **Non-obvious:** It is not the title, main thesis, a section heading restated in prose, common domain advice, a familiar aphorism, or something most attentive readers would immediately notice.
2. **Consequential:** Believing it changes a decision, prediction, mental model, or useful question. Mere novelty is insufficient.
3. **Derived:** Explain the short reasoning chain from source evidence to the insight. A quotation, anecdote, statistic, or author assertion alone is not an insight.
4. **Well-supported:** The cited passage genuinely supports the claim without cherry-picking, and meaningful counterevidence elsewhere in the source has been considered.
5. **Bounded:** State the conditions, scope, or uncertainty that keep the claim from becoming an overgeneralization.
6. **Locatable:** A reader can navigate directly to the supporting material using the supplied locator.

Use this internal scoring check after the gates:

- non-obviousness: 0–2
- consequence: 0–2
- strength of derivation: 0–2
- evidential support: 0–2
- specificity and boundaries: 0–2

Report a candidate only when it scores at least 8/10, with a 2 for both non-obviousness and evidential support. When uncertain, omit it. Do not relax the threshold to ensure the response contains something.

Reject observations that are merely:

- summaries, themes, definitions, or the author's headline conclusions;
- memorable quotes, examples, facts, statistics, or contrarian phrasing with no derived implication;
- generic advice that could have been written without inspecting this source;
- speculative leaps supported by only one ambiguous passage;
- several restatements of the same underlying insight.

## Source locators

Attach the tightest locator the available format supports:

- YouTube or other video: timestamp or narrow timestamp range, plus chapter/segment when present; include a timestamped link when possible.
- Podcast or audio: timestamp range and episode/segment title; identify the transcript used when relevant.
- Book or ebook: chapter and section plus page for the specified edition. If stable pages do not exist, use chapter/section and a short paragraph-opening phrase or ebook location.
- Article or web page: section heading and paragraph number within that section, plus a short paragraph-opening phrase and link.
- PDF: printed page number when present and PDF page index when they differ, plus section or heading.

Never invent precision. If the source only permits a coarse locator, say so. Use a very short evidence fragment only when it helps the reader verify the location; prefer paraphrase and never reproduce long copyrighted passages.

## Output

Lead with one sentence stating the result and the inspected scope. Return at most five insights by default, ranked strongest first; fewer is better.

For each qualifying insight, provide:

- **Insight:** one precise, standalone claim.
- **Why it is non-obvious:** what a superficial reading would miss.
- **Derivation:** the compact evidence-to-claim reasoning chain, clearly separating source claims from inference.
- **Source anchor:** the exact locator and link when available.
- **Boundary:** when the insight may not hold or what remains uncertain.

Do not show scores or rejected candidates unless the user asks. Do not pad the list with near-misses.

If none qualify, say **No qualifying insights found.** Briefly name the inspected scope and the main reason the strongest candidates failed, such as being explicit summaries, familiar advice, weakly supported, or not consequential. Do not substitute a summary unless the user asks for one.
