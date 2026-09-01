# Baseline prompts

Three fixed prompts for reviewing this guide against a new model. See
"Reviewing this guide against a new model" in `SKILL.md` for what to do with the
output.

They cover the three length modes the guide calibrates to, because the tells
differ by length. One is Swedish, so patterns 31 to 35 get exercised too.

Keep the wording frozen. The point is to compare models, not prompts. If a
prompt has to change, note it in the log below and treat everything before the
change as a separate baseline.

## How to run them

**Run each one in a clean context.** No CLAUDE.md, no skills loaded, no prior
turns, no system prompt of your own. A fresh chat on claude.ai, or a directory
with no CLAUDE.md in it.

This matters more than it sounds. Stefan's global CLAUDE.md says "answer in
Swedish" and "keep answers concise", and both instructions change the output
enough to invalidate the comparison. You are measuring what the model does when
nobody has told it anything.

**Do not mention this skill, humanizing, AI writing patterns, or "write
naturally".** Any of those turn the test into a test of instruction following.

Paste the prompt, take the first response, change nothing. A second attempt is a
different measurement.

---

## 1. Long, English, personal

> Write a 900 word blog post, first person, about a side project I paused after
> three weeks. It was a price index for the Swedish second hand board game
> market, built to find out whether there was money in buying and selling used
> games. The answer turned out to be no: the median sale was 130 kronor, only
> about half of everything listed sells at all, and almost nothing published
> after 2020 changes hands in any volume. Cover what I built, what the data
> said, and what I would do differently.

Exercises: significance inflation, manufactured suspense, generic positive
conclusions, rule of three, em dashes, corporate compounds, whether it can hold
a first person voice without narrating its own structure.

## 2. Short, Swedish, social

> Någon har kommenterat mitt LinkedIn-inlägg om att jag lämnat anställningen för
> att bygga eget: "Vad kul Stefan! Vi hörs snart, jag är nyfiken på vad du
> bygger." Skriv mitt svar.

Exercises: Swedish LinkedIn voice, over-formal register, translated English
idiom, connector stacking, imported dash typography. Also the length
calibration: a good answer is one or two lines, and producing a paragraph is
itself the finding.

## 3. Functional, English, documentation

> Write the "Getting started" section of a README for a small command line tool
> that reads a CSV of expenses and prints a monthly summary. It runs on Node,
> installs with one command, and has a handful of subcommands.

Exercises: signposting, fragmented headers, boldface overuse, inline-header
vertical lists, title case in headings, decorative emojis, filler around code
blocks.

---

## Log

Record every review here. Model, date, and what changed in the guide as a
result. A pattern retired in one generation can return in the next, and knowing
when it was last seen is the difference between a judgement and a guess.

| Model | Date | Patterns that fired | Patterns that stayed quiet | Changes made |
|---|---|---|---|---|
| | | | | |

No baseline has been recorded yet. The first run establishes one, so run these
against the current model before the next release, not only after it. A single
column of results says nothing about what changed.
