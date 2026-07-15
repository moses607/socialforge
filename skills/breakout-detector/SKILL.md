---
name: breakout-detector
description: Finds outlier "breakout" content in a niche before it saturates by normalizing engagement against each account's own baseline, then isolating the format, angle, or sound driving the spike. Use when someone asks "what's working in my niche," wants to spot trends early, or needs to separate real breakouts from big-account noise. Trigger on outlier/breakout/trend-spotting/"what should I make" requests. Works with any capable model.
---

# Breakout Detector

Big accounts get big numbers on everything — that is baseline, not signal. A true breakout is a post that beats *its own account's* normal performance by a wide margin, because that gap is the market voting for a specific idea before the algorithm saturates it. This skill has no live data of its own: the user (or a paired search/scraper tool) supplies recent posts with per-account stats, and you turn that raw list into ranked, normalized breakout patterns plus a brief to make your own version fast. Speed of detection beats precision — a 70%-confidence pattern acted on this week beats a perfect one found after saturation.

## 1. Gather and normalize
1. Collect 30-100 recent posts (last 7-30 days) across 10+ accounts in the niche. For each, require: account follower count, that account's typical/median views, this post's views, and likes+comments+shares+saves.
2. Compute the **Outlier Score** two ways and keep the higher:
   - `View Multiple = post views ÷ that account's median views` (best signal; needs per-account baseline).
   - `Reach Ratio = post views ÷ follower count` (fallback when you lack an account baseline).
3. Flag as breakout candidate if View Multiple ≥ 3x OR Reach Ratio ≥ 5x. Discard anything under 2x — it's baseline.
4. Kill false positives: drop posts inflated by paid ads, a collab with a far-bigger account, or a one-off news spike unrelated to the niche.

## 2. Isolate the driver
For each candidate, name the ONE variable most responsible. Score every candidate across:
1. **Format** — carousel, talking-head, green-screen, listicle, B-roll voiceover, text-on-screen.
2. **Angle/hook** — contrarian take, "I was wrong about X", before/after, mistake-confession, us-vs-them.
3. **Sound/audio** — trending sound ID, original VO, specific song. Note if the same sound repeats across candidates.
4. **Structure** — hook <2s, payoff timing, loop, open-loop CTA.
Cluster candidates that share a driver. A pattern only counts when 3+ different accounts hit outlier scores using the same driver — one viral post is luck, three is a pattern.

## 3. Score breakout potential
Rate each pattern 1-5 on three axes, then multiply:
- **Novelty** (is it still early, few imitators?) × **Proven demand** (how many accounts + how high the multiples?) × **Your execution fit** (can YOU ship this in <48h with your skills/assets?).
Score of 45+ (of 125) = make it now. Below 20 = skip; either saturated or off-fit.

## Output template
```
NICHE: <niche> | Window: <dates> | Posts analyzed: <n>

TOP BREAKOUT PATTERNS (ranked)
1. <Pattern name> — Driver: <format/angle/sound>
   Evidence: <n> accounts, avg <Xx> outlier score, e.g. @acct 8.2x
   Score: Novelty _/5 × Demand _/5 × Fit _/5 = __/125
   Why it's spiking: <1 line, first-principles>

MAKE-YOUR-VERSION BRIEF (pattern #1)
- Hook (first 2s): <copy-ready line>
- Format/shot list: <specifics>
- Sound/audio: <ID or type>
- Your angle twist: <how you make it yours, not a clone>
- Ship-by: <date, within 48h>

SKIP LIST: <saturated or off-fit patterns + why>
```

## Platform variants
- **TikTok/Reels/Shorts**: View Multiple is king; watch sounds — a shared trending sound across candidates is the strongest early signal. Saturation window is 3-10 days.
- **YouTube**: use views ÷ channel median and outlier thumbnails/titles; breakouts live longer (weeks), so novelty decays slower.
- **X/Threads**: use impressions ÷ follower count; driver is usually angle/hook, not format. Decay is hours.
- **LinkedIn/Instagram feed**: saves and shares outweigh likes; normalize on those.

## Rules
- Never rank by raw views or follower count — always normalize to the account's own baseline, or you'll just rediscover big accounts.
- A pattern needs 3+ independent accounts hitting outlier scores; one hit is noise.
- Detect the driver, not the topic — copying the topic saturates; copying the format/angle transfers.
- Act inside the saturation window (days, not weeks) or the edge is gone — favor speed over a perfect read.
- Always add a twist so your version isn't a clone; the algorithm punishes duplicates.
- Demand you get fresh input data each run — this skill scores what it's fed and never claims live knowledge.
