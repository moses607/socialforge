---
name: analytics-interpreter
description: Turns raw platform analytics into a funnel diagnosis instead of a data dump. It reads every metric as evidence about ONE stage of the growth funnel, locates the single biggest leak, and prescribes the fix. Use when someone shares metrics/insights, asks "what do these numbers mean", "why are my views low", or "why isn't this growing". Works with any capable model.
---

# Analytics Interpreter

Metrics are not a scoreboard; they are a diagnostic X-ray of one funnel: Distribution -> Hook -> Body -> Conversion -> Amplification. Every number is evidence about exactly one stage. Growth stalls because ONE stage leaks, not because "everything is bad." Your job is not to summarize the dashboard — it is to name the single leak that, if fixed, unlocks the most upside, and ignore everything else. Vanity metrics (likes, followers, total views) describe the past; rate metrics (hook rate, retention, saves-per-view) predict the future. Diagnose rates.

## 1. Map each metric to what it REVEALS

1. Impressions / reach -> DISTRIBUTION. How many the algorithm tested you on. Low reach = the algorithm killed it early (usually a hook or early-retention problem, not a reach problem).
2. Hook rate / 3s-view rate (views ÷ impressions) -> HOOK QUALITY. Below ~30% weak, 30-45% average, 45%+ strong. This is the first gate.
3. Average watch time & retention curve -> BODY/CONTENT QUALITY. For short video, watch-time ratio (avg watch ÷ length) above ~0.8 is strong; full watch or rewatch (>1.0) triggers pushes.
4. CTR (on titles/thumbnails, YouTube/blogs) -> PACKAGING. 2-4% baseline, 5%+ strong, sub-2% weak.
5. Saves & shares -> VALUE + IDENTITY. THE growth signals. Save = "useful to future me." Share = "this represents me." Target saves+shares ≥ 1-2% of views.
6. Follows-per-view -> PROFILE + CONTENT FIT. Are viewers converting to subscribers.
7. Comments -> RESONANCE. Emotional or debate-worthy enough to react.

## 2. Read the retention curve — the drop tells you what to fix

1. Cliff in first 1-3s -> hook fails / mismatch between hook promise and thumbnail-or-first-frame. Fix the opening.
2. Steady slow decline -> normal; healthy content loses viewers gradually. Leave it.
3. Sudden mid-video drop -> a specific dead moment: slow setup, tangent, no payoff yet. Cut it.
4. Flat / rising line -> loops, open loops, or payoff pulling viewers through. Do MORE of this.
5. Compare the CURVE, not the average — two videos with equal avg watch time can have opposite fixes.

## 3. Find the ONE leak, then stop

1. Walk the funnel top-down. Find the FIRST stage below benchmark — that is the binding constraint.
2. Reach low + hook rate low -> HOOK leak. Reach low + hook fine -> topic/niche-fit or account-trust leak.
3. Hook fine + retention drops -> BODY leak (pacing/payoff). Hook + retention fine but low follows/saves -> CONVERSION leak (weak CTA, no reason to follow, no takeaway to save).
4. Everything decent but flat growth -> AMPLIFICATION leak (not shareable/saveable — no identity or utility payload).
5. Name exactly ONE leak. Fixing the top leak moves everything downstream; fixing downstream while the top leaks wastes effort.

## Output template
```
FUNNEL DIAGNOSIS
- Distribution (reach/impressions): [n] — [healthy/leaking]
- Hook (3s / hook rate): [n]% — [vs ~40% benchmark]
- Body (retention / avg watch): [n]% — curve shape: [cliff/decline/flat]
- Conversion (follows-per-view, saves): [n] — [healthy/leaking]
- Amplification (shares+saves per view): [n]% — [healthy/leaking]

BIGGEST LEAK: [stage] — [one sentence why, citing the number]

THE FIX: [one concrete change to make on the next post]
Expected signal to watch: [which metric should move]
```

## Platform variants
- TikTok/Reels/Shorts: hook rate + watch-time ratio dominate; saves/shares are the amplifiers.
- YouTube long-form: CTR × avg-view-duration is the algorithm's core; a great CTR with low retention gets throttled.
- Instagram feed/carousels: saves and sends are the ranking signal; reach follows them.
- X/LinkedIn: profile clicks, dwell/expands, and reposts over raw impressions.

## Rules
- Name ONE leak. A diagnosis with three problems is not a diagnosis.
- Always diagnose RATES; never conclude from raw totals or follower count.
- Read the retention CURVE shape, not just average watch time.
- Treat saves and shares as the leading indicators of reach — reach is the lagging result.
- Low reach is almost never a "reach problem" — it is the algorithm reacting to a hook or early-retention leak.
- If a benchmark is unknown, compare the post against the account's own median, never against zero.
