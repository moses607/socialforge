---
name: viral-script-generator
description: Writes short-form video scripts engineered for watch-time and completion, not just clever lines. Produces a shot-by-shot table pairing spoken lines, on-screen text, and B-roll direction with retention beats every 5-7 seconds. Use when the user asks to "write me a script", "turn this idea into a video", or mentions a reel, short, story, TikTok, or video. Trigger on script/video/reel/short/story requests. Works with any capable model.

---

# Viral Script Generator

Retention is the only metric that compounds. The algorithm promotes what people finish and rewatch, so every line must earn the next three seconds. A script is not prose read aloud — it is a sequence of engineered beats where spoken audio, on-screen text, and visual all carry different jobs at once. Write for the scrubbing thumb: assume the viewer decides to stay or swipe every few seconds, and give them a reason each time.

## 1. Build the spine (HOOK → re-hook → escalation → payoff → CTA)
1. HOOK (0-3s): state the stakes or the promise in the first spoken breath. Lead with the result, the contradiction, or the tension. On-screen text mirrors a sharper version of the hook so muted viewers still get it.
2. RE-HOOK (3-8s): pay off why they should trust you or add context that raises stakes ("I tested this for 30 days"). Never restate the hook — advance it.
3. ESCALATION: stack 3-5 value beats, each raising tension or specificity. Plant an open loop early ("the third one broke my assumptions") and close it near the end.
4. PAYOFF: deliver the promised result. This is the emotional peak — make it concrete and visual.
5. CTA: single ask, tied to the payoff.

## 2. Engineer retention beats
1. Pattern interrupt every 5-7s: cut angle, zoom punch, B-roll swap, sound effect, or text pop. Monotony is the #1 drop-off cause.
2. Open loops: tease something you resolve later. Never leave a loop unclosed — it kills trust.
3. Contrast pacing: alternate fast dense lines with one slow deliberate line for emphasis. Vary sentence length.
4. On-screen text as a second channel: text = keyword or punchline, audio = full sentence. They should never be identical.
5. Kill dead air: trim every "so", "basically", "um". First frame must be motion or a face mid-sentence, never a slow intro.

## 3. Pick the arc
- **Before/after transformation**: show the pain state, the turn, the result. Best for tutorials, fitness, product.
- **Myth-bust**: "You've been told X. It's wrong. Here's why." High save rate.
- **Listicle**: "3 things..." — numbered, each item a beat. Promise count in hook, deliver fast.
- **Story/POV**: first-person tension, a twist, a lesson. Highest completion when the payoff reframes the opening.

## Output template
```
Idea: <one line> | Arc: <arc> | Target length: <Xs> | Platform: <x>

| # | Time | Spoken line | On-screen text | Visual / B-roll | Beat type |
|---|------|-------------|----------------|-----------------|-----------|
| 1 | 0-3s | <hook line> | <bold hook text> | <shot direction> | HOOK |
| 2 | 3-8s | <re-hook> | <keyword> | <cut/zoom> | RE-HOOK + open loop |
| 3 | 8-14s| <value 1> | <keyword> | <b-roll> | pattern interrupt |
| ...| ... | ... | ... | ... | escalation |
| n-1| ... | <payoff> | <result text> | <peak visual> | PAYOFF + close loop |
| n | ... | <cta> | <cta text> | <face to cam> | CTA |

Caption: <hook-echoing caption + 3-5 tags>
```

## Platform variants
- **TikTok/Reels**: 21-34s hits the sweet spot; native captions; trend audio under a voiceover.
- **YouTube Shorts**: front-load harder — first 1s is do-or-die; can run to 45-60s if payoff justifies.
- **Stories**: 15s segments, one idea each, tap-forward friendly, sticker CTA.

## Rules
- Never ship the first hook. Generate 15+, ship the best 1-3. The hook must be true to the payoff or retention and trust collapse.
- Spoken line and on-screen text carry different loads — never duplicate them word-for-word.
- One idea per video. If it needs two, it's two videos.
- Every open loop must close. No exceptions.
- Cut the intro. Start mid-action, first frame in motion.
- Match CTA aggression to the platform: soft ("comment X for the link") for reach, hard ("link in bio") for conversion. Comment-bait a genuine question, never a fake one.
