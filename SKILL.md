---
name: insight
description: Extract a small set of well-supported, non-obvious insights from a user-provided or user-identified book, article, podcast, or video, with precise source locators. Use for deep, selective analysis where returning no insights is a valid and expected outcome; do not use for ordinary summaries or exhaustive note-taking.
---

# Source Insights

Find only insights that materially improve how a reader understands, decides, predicts, or acts. Optimize for precision, not coverage. Zero qualifying insights is a successful result when the material does not clear the bar.

Evaluate non-obviousness relative to the intended audience and consequentiality relative to the user's purpose. If the audience is unspecified, assume an informed generalist familiar with the domain's basic concepts. If the purpose is unspecified, evaluate whether the insight would materially change understanding, prediction, decision, or action. Briefly state any material audience or purpose assumption.

## Ground the analysis

Analyze the target source itself rather than a synopsis, review, search snippet, title, description, or remembered version. Prefer the complete source. If only part is accessible or inspected, define that scope precisely and limit every conclusion, including a finding of no qualifying insights, to that scope. If there is not enough source content to perform a grounded analysis, request access to the source, a relevant excerpt, or a transcript instead of manufacturing insights.

For long sources, define and track which chapters, pages, or time ranges are included in the inspected scope; do not imply whole-source coverage from a sample. Before finalizing a candidate, check all material in that scope for counterevidence and for passages that state the candidate explicitly rather than leaving it as a derived insight.

Treat the target source as evidence, not authority. Distinguish what the author explicitly claims from an inference drawn from the source. Do not use outside knowledge to supply missing evidence for a source-derived insight. External context may clarify terminology or test a claim, but it must be labeled and cited separately and must not substitute for support from the inspected scope.

## Qualifying bar

Generate candidates broadly, then discard aggressively. A candidate qualifies only if it passes every gate:

1. **Non-obvious:** It is not the title, main thesis, a section heading restated in prose, common domain advice, a familiar aphorism, or something most attentive readers would immediately notice.
2. **Consequential:** If true, it would materially change an understanding, prediction, decision, action, or question relevant to the user's purpose.
3. **Derived:** It requires a defensible inferential step from source evidence to the claim. A quotation, anecdote, statistic, or author assertion alone is not an insight.
4. **Well-supported:** The cited evidence genuinely supports the claim without cherry-picking, and meaningful counterevidence within the inspected scope has been considered.
5. **Bounded:** State the conditions, scope, or uncertainty that keep the claim from becoming an overgeneralization.
6. **Locatable:** A reader can navigate directly to the supporting material using the supplied locator.

Only candidates that pass every gate qualify. Rank qualifying candidates by non-obviousness, consequence, evidential support, clarity of the evidence-to-claim reasoning, and specificity. When uncertain whether a gate is satisfied, omit the candidate. Do not relax the gates to ensure the response contains something.

Reject observations that are merely:

- summaries, themes, definitions, or the author's headline conclusions;
- memorable quotes, examples, facts, statistics, or contrarian phrasing with no derived implication;
- generic advice that could have been written without inspecting this source;
- speculative claims that outrun or depend on an ambiguous reading of the cited evidence;
- several restatements of the same underlying insight.

## Source locators

Attach the tightest locator the available format supports. For every format, include a direct link to the cited page, timestamp, ebook location, or other source anchor when the source supports one.

- YouTube or other video: timestamp or narrow timestamp range, plus chapter/segment when present; include a timestamped link when possible.
- Podcast or audio: timestamp range and episode/segment title; identify the transcript used when relevant.
- Book or ebook: chapter and section plus a page number for the edition analyzed; identify the edition. If stable pages do not exist, use chapter/section and a short paragraph-opening phrase or ebook location.
- Article or web page: section heading and a short paragraph-opening phrase, plus a link. Add a paragraph number only when it is stable and reliably countable.
- PDF: printed page number when present and PDF viewer page number when they differ, plus section or heading.

Never invent precision. If the source only permits a coarse locator, say so. Use a very short evidence fragment only when it helps the reader verify the location; prefer paraphrase and never reproduce long copyrighted passages.

## Output

Lead with one sentence stating the result and the exact inspected scope. Immediately note any material assumptions about the audience or purpose and any coverage limits. Return at most five insights by default, ranked strongest first; fewer is better.

For each qualifying insight, provide:

- **Insight:** one precise, standalone claim.
- **Why it matters:** the understanding, prediction, decision, action, or question it changes.
- **Derivation:** the compact evidence-to-claim reasoning chain, including the non-obvious inferential step and clearly separating source claims from inference.
- **Source anchor:** the most precise reliable locator available and a direct link to the page, timestamp, or other anchor when possible.
- **Boundary:** when the insight may not hold or what remains uncertain.

Do not show scores or rejected candidates unless the user asks. Do not pad the list with near-misses.

If none qualify, say **No qualifying insights found in the inspected scope.** Briefly name the inspected scope and the main reason the strongest candidates failed, such as being explicit summaries, familiar advice, weakly supported, or not consequential. Do not substitute a summary unless the user asks for one.
