---
name: growth-orchestrator
description: The coordinator for SocialForge — routes a social-media goal to the right skills in the right order and runs them as an end-to-end workflow. Use when the user gives a broad growth goal ("grow my account", "launch on TikTok", "go viral", "plan my month", "I have a video, do everything"), or isn't sure which skill they need. Trigger on any multi-step social-growth request. Works with any capable model.
---

# Growth Orchestrator

Individual skills are power tools; the orchestrator is the workflow that points them at a goal in sequence, passing each skill's output into the next. It turns "help me grow" into a concrete pipeline with a deliverable at the end.

## First: diagnose the goal

Classify the request into one of the standard workflows, and gather the minimum inputs (niche, platform(s), current size, the asset if any). Don't over-ask — start with what's given and fill gaps as you go.

## Standard workflows (skill chains)

- **New account / from scratch:**
  `onboarding-brand-brief` → `audience-bullseye` → `channel-competitor-analysis` → `content-strategy-engine` → `hook-machine` → `viral-script-generator`
- **"I have one long video, do everything":**
  `repurpose-master` → `hook-machine` (per clip) → `cross-platform-adapter` → `visual-idea-generator` → posting schedule
- **"Make this specific post go viral":**
  `channel-competitor-analysis` (of top performers in niche) → `hook-machine` → `viral-script-generator` → `visual-idea-generator`
- **Ride a trend now:**
  `trend-jacker` → `hook-machine` → `viral-script-generator` (fast lane, ship same day)
- **Monthly plan:**
  `audience-bullseye` → `content-strategy-engine` → `campaign-builder` → cadence
- **"Why isn't this working?":**
  `analytics-interpreter` → `performance-optimizer` → `hook-machine` / `content-strategy-engine` (fix the weakest link)
- **Launch/series/challenge:**
  `campaign-builder` → `content-strategy-engine` → `viral-script-generator` → `engagement-booster`

## Method

1. **Route.** Pick the workflow; state the chain you'll run and the final deliverable.
2. **Run in sequence, pass context forward.** Each skill consumes the prior output (persona → pillars → hooks → scripts). Don't restart from zero at each step.
3. **Gate on quality.** After hooks and scripts, apply the ship-only-4s-and-5s bar (see `hook-machine`). Weak link → loop that one skill, don't proceed.
4. **Deliver + measure.** End with a concrete artifact (calendar, script pack, campaign) and the metric to watch. Feed real results back into `performance-optimizer` next cycle.

## Output template

```
## Growth plan: <goal>
Workflow: <named chain>
Inputs used: <niche / platform / size / asset>

### Pipeline
Step 1 — <skill> → <output>
Step 2 — <skill> → <output> (uses step 1)
...

### Deliverable
<the final artifact>

### Metric to watch + next-cycle loop
<the one number; what to run next based on it>
```

## Rules

- Always name the chain and the final deliverable before running it — no aimless brainstorming.
- Pass context forward; never make a later skill re-derive what an earlier one already produced.
- One weak link kills the funnel. Gate after hooks/scripts and loop the weakest step rather than shipping it.
- Match ambition to inputs — a from-scratch account gets foundations first (persona, pillars), not a viral moonshot.
- Close the loop: every plan ends with a metric and what to run next cycle.
