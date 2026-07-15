---
name: channel-competitor-analysis
description: Reverse-engineer any creator, channel, profile, or single viral post to extract the hooks, formats, content pillars, posting cadence, engagement patterns, and exploitable weaknesses behind their growth. Use when the user wants to analyze a competitor/account/video, understand why something went viral, find gaps to attack, or model a winning channel. Trigger on "analyze this profile/channel/video", competitor research, or "why did this blow up". Works with any capable model.
---

# Channel & Competitor Analysis

Growth leaves fingerprints. Every channel that works is running a repeatable system — a few pillars, a hook style, a format, a cadence — and you can read it off their public output. The goal is not to copy; it's to find the **pattern they're exploiting** and the **gap they're leaving open** for you.

## Inputs

Ask for (or work with what's given): the profile/handle, 5-20 of their recent posts (ideally their top performers), and follower/engagement numbers if available. If you only have a URL, work from titles, hooks, thumbnails, and visible metrics.

## Method

1. **Separate outliers from baseline.** Rank their posts by engagement relative to *their own* average. The 2-3× outliers are the signal — that's what the audience actually wants. The baseline is filler.
2. **Decode the outliers** on five axes:
   - **Hook** — the opening move and archetype (see `hook-machine`).
   - **Format** — talking-head, listicle, story, tutorial, reaction, B-roll+VO.
   - **Pillar** — the recurring topic/theme it belongs to.
   - **Emotion** — what it makes the viewer feel (status, fear, curiosity, belonging, aspiration).
   - **Structure** — hook → escalation → payoff → CTA; where retention is engineered.
3. **Map the pillars.** Cluster all posts into 3-5 content pillars; note the % of output and % of total engagement per pillar. The high-engagement/low-output pillar is an underexploited vein.
4. **Read the cadence & funnel.** Posting frequency, best-performing times, and how they convert attention (link in bio, series, lead magnet, product).
5. **Find the weaknesses (your opening).** Where are they weak or absent? Common gaps: no strong hooks, no series/retention loop, ignoring a platform, weak CTA, a pillar their audience loves but they underserve, poor production, or a tone that alienates a sub-segment.

## Output template

```
## Analysis: <channel/creator>
Baseline vs outliers: avg engagement <x>; outliers <list top 3 + their multiple>

### What's working (their winning system)
Pillars (share of output / share of engagement): <table>
Hook style: <..>  | Dominant format: <..>  | Core emotion: <..>
Cadence & best times: <..>  | Conversion path: <..>

### Why the outliers hit
<per top post: hook + structure + emotion, 1-2 lines each>

### Their weaknesses = your openings
<3-5 specific, exploitable gaps>

### Attack plan for you
<3 concrete content moves that use their gap + your edge>
```

## Rules

- Analyze outliers, not averages — the average post tells you what didn't work.
- Model the system, don't clone the posts. Copying a viral video a week late loses; stealing its *mechanism* wins.
- Always end with an attack plan — analysis without an action is trivia.
- Separate "what they do" from "what actually drives their engagement" — creators are often wrong about their own hits.
- Note production floor: if their weakness is low effort, your opening is craft; if it's craft, your opening is speed/volume or a sharper niche.
