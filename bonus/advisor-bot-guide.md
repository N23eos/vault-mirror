# Bonus — Advisor Bot Guide

## Goal

Turn the digital-advisor prompt into a bot you can actually talk to. This is a
guide for the human (with agent help), not an analysis module. It is
stack-agnostic: pick whatever you already use.

**Requires:** `Analysis/digital-advisor.md` exists (run `bonus/digital-advisor.md` first).

## Option A — Zero setup: a project/custom bot in your chat app

Most chat products let you save a system prompt: Claude Projects, ChatGPT
custom GPTs/projects, or a saved character in any local UI. Paste the advisor
prompt as the system prompt / project instructions. Optionally attach
`09-executive-summary.md` as project knowledge. Done in five minutes.

**Privacy note:** the prompt is a distilled psychological profile. Only put it
in services you already trust with your notes' content.

## Option B — Local model

Use a local runner (Ollama, LM Studio, llama.cpp or similar) and set the
advisor prompt as the system prompt. Nothing leaves your machine. Quality
depends on the local model — prefer the largest one your hardware runs.

## Option C — Messenger bot

Any framework that connects an LLM API to Telegram/Discord/Slack works. The
essentials regardless of stack: the advisor prompt goes in as the system
prompt; keep conversation history in the context window; add a periodic
reminder message re-injecting the prompt if the framework truncates context.

## Keeping it current

The advisor decays as your life moves on. Refresh path: re-run the analysis
(or the incremental modules you care about) → regenerate
`Analysis/digital-advisor.md` → swap the prompt. A quarterly refresh is
plenty for most people.

## What NOT to do

- Don't give the bot write access to your vault.
- Don't treat it as therapy. It is a well-informed mirror, not a clinician —
  if the analysis surfaced heavy material, a human professional is the tool.
- Don't share the advisor prompt itself; it's the most concentrated personal
  document this toolkit produces.
