# Insight

`insight` is a Codex skill for extracting a small number of genuinely non-obvious, consequential insights from books, articles, podcasts, videos, and other source material.

It prioritizes grounded analysis, precise source anchors, explicit boundaries, and intellectual honesty. If the source does not contain anything that clears the bar, returning no insights is the correct result.

## What makes it different

Most summaries repeat a source's main thesis, memorable facts, or familiar advice. `insight` looks for derived claims that can materially improve how you understand, decide, predict, or act.

Read the full skill definition: [$insight](./SKILL.md).

## Usage

Just point it at a source (e.g. book, article, youtube video, podcast) that you want to extract insights from.

## Examples

### Example 1: Analyze a YouTube video
```text
$insight https://www.youtube.com/watch?v=zdbVtZIn9IM
```

### Example 2: Analyze a book chapter by chapter

```text
Use $insight for every chapter in the attached book.

You may use subagents, but each agent must focus on exactly one chapter at a time.

Return a list of chapters, with a nested list of qualifying insights for each chapter.

<Book attached>
```

## Model choice matters

This skill asks the model to distinguish obvious observations from genuinely useful insights, connect evidence across a source, consider counterevidence, and keep claims properly bounded. Stronger reasoning models therefore produce noticeably better results.

For example, in current usage, GPT-5.6 Luna often surfaces fairly obvious or generic takeaways, whereas GPT-5.6 Sol is much more likely to identify deeper, more useful, and better-supported insights—particularly when working with long or complex source material.

## License

[MIT License](./LICENSE).
