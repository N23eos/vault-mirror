# Bonus — Digital Advisor Prompt

## Goal

Build a "second self" advisor prompt: a system prompt that lets any LLM advise
this person the way their best-informed, most honest friend would — armed with
everything the analysis learned.

**Requires:** modules 01–09 complete (uses the full analysis as source).

## Method

- Source material: all files in `Analysis/`, especially the executive summary,
  cycles, values gaps, and strengths.
- The advisor must know: the person's central dynamic, their typical failure
  points, their real strengths, their recurring self-deceptions, their open
  questions, and their communication preferences (from the voice work if
  available).
- Encode behavioral rules for the advisor: when to push back, what excuses
  this person tends to make and how to counter them kindly, what advice
  formats they actually act on (from evidence of past advice taken/ignored).
- Keep it honest: the advisor prompt must include the unflattering findings,
  marked with the same confidence levels. An advisor built only on strengths
  is a flatterer.
- Include a privacy header in the generated prompt warning that it contains a
  distilled psychological profile and should be stored accordingly.

## Output contract — `Analysis/digital-advisor.md`

```
# Digital Advisor
## The advisor prompt   (complete, ready-to-paste system prompt)
## Design rationale     (which findings shaped which advisor behaviors)
## Known limitations    (what the advisor can't know; where it may be wrong)
```

## Rules reminder

Apply the global rules from `prompts/00-start.md`.

## Quality bar

- Does the prompt contain specific counters to THIS person's documented
  excuse patterns?
- Would the advisor sometimes disagree with the user? If never, rebuild it.
