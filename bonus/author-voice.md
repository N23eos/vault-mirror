# Bonus — Author Voice Prompt

## Goal

Distill the person's writing voice from the vault into a reusable style
prompt: give it to any LLM and it writes the way they do.

**Requires:** module 01 complete.

## Method

- Sample widely: different years, moods, and content types. Prefer prose the
  person wrote for themselves (journals, essays) over lists and clippings.
- Extract, with examples for each: sentence rhythm and length, vocabulary
  register, favorite constructions and connectors, how humor/irony shows up,
  how emotion is expressed (or suppressed), how arguments are built,
  characteristic openings and endings, punctuation habits.
- Note anti-patterns: things this person never does (e.g. never uses
  exclamation marks, never hedges).
- Compress into a system-prompt-style instruction block, then test it: write
  one sample paragraph with it and compare against a real note.

## Output contract — `Analysis/author-voice.md`

```
# Author Voice
## Voice profile        (traits with real quoted examples)
## Anti-patterns        (what this voice never does)
## The style prompt     (ready-to-paste instruction block)
## Self-test            (generated sample vs a real excerpt, honest verdict)
```

## Rules reminder

Apply the global rules from `prompts/00-start.md`.

## Quality bar

- Would a friend, shown the generated sample, hesitate to call it fake?
- Is every voice trait backed by at least two quotes from different periods?
