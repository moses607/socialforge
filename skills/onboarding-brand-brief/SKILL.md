---
name: onboarding-brand-brief
description: First-run setup that captures a creator's foundation — niche, positioning, offer, platforms, and voice — into a reusable BRAND BRIEF block the other SocialForge skills read from. Includes a voice-training step that extracts tone, lexicon, and rhythm from the creator's own posts (or admired creators) so generated content sounds like a person, not a model. Use when the user first opens SocialForge, or says "set up my brand", "set up my profile", "train my voice", or is onboarding. Trigger on any first-run or profile-setup intent. Works with any capable model.
---

# Onboarding Brand Brief

Everything downstream — hooks, personas, calendars, captions — degrades to generic mush without a foundation the model can anchor on. A brand brief is not branding fluff; it is a compression of five decisions (who you serve, why you, what you sell, where, and how you sound) into a block short enough to prepend to every generation. Extract it once, reuse it forever. The single highest-leverage step is voice training: a model that has read five of the creator's real posts stops writing "in today's fast-paced world" and starts writing like them.

## Method: interrogate the five pillars
Ask these in order. One question at a time. Push back on vague answers — "fitness" is not a niche, "busy moms who want to lift heavy without a gym" is.
1. **Niche + sub-niche.** Force specificity. Broad niche = the room; sub-niche = the corner they own. Reject anything you could put on a billboard for a competitor.
2. **Positioning / unique angle.** Finish this sentence with them: "Unlike everyone else in [niche], I ___." If they can't, probe their contrarian take, origin story, or unfair advantage.
3. **Offer + primary goal.** What is the money or growth event? Followers, email leads, product sales, bookings? Name ONE primary goal and the metric that proves it. Secondary goals get logged but never drive the strategy.
4. **Platforms.** Where do they post now and where do they want to. Rank them. Downstream skills adapt format per platform.
5. **Voice attributes.** Pull 3 adjectives, but make them earn it — "professional" is banned. Push for tension pairs like "blunt but warm" or "nerdy but irreverent".

## Method: voice training from real posts
1. Ask for 3-5 of their best-performing or favorite posts — their own, or admired creators they want to sound like (flag which).
2. Extract three layers explicitly: **tone** (emotional default — deadpan, hyped, tender), **lexicon** (recurring words, slang, jargon, signature phrases, emoji habits), **rhythm** (sentence length, one-liners vs paragraphs, use of line breaks, punctuation quirks).
3. Derive a **do-words / don't-words** list: words that sound like them, and words that would break the illusion (corporate filler, hashtag-speak, AI tells like "delve", "elevate", "unlock").
4. Write one 2-sentence sample in their voice and ask "does this sound like you?" Iterate until yes. Do not finalize the brief on an unconfirmed voice.

## Output template
```
=== BRAND BRIEF ===
Niche: <broad> > <sub-niche>
ICP one-liner: <the one specific person served, in a sentence>
Positioning: Unlike others in <niche>, I <unique angle>.
Voice attributes: <adj1>, <adj2>, <adj3>
Do-words: <word, word, phrase, emoji habit>
Don't-words: <banned filler / AI tells / off-brand terms>
Rhythm: <sentence length + structure signature>
Platforms (ranked): <1>, <2>, <3>
Primary goal: <goal> | Metric: <the number that proves it>
Secondary goals: <optional>
=== END BRIEF ===
```

## Platform variants
- **Short-form video (TikTok/Reels/Shorts):** voice attributes should include a spoken-cadence note — how they'd say it out loud, not write it.
- **LinkedIn/X:** capture a "credibility marker" (role, result, receipts) since positioning leans on authority.
- **Instagram/Pinterest:** log an aesthetic note (visual mood) alongside voice; the brief feeds caption tone, not just copy.

## Rules
- One question at a time. A wall of 10 questions gets skimmed and answered lazily — the brief is only as good as the answers.
- Reject vague niches and banned adjectives ("professional", "authentic", "high-quality") on sight — make them replace the word with a specific one.
- Never finalize until the voice sample passes the "sounds like me" test; an unconfirmed voice poisons every downstream generation.
- The brief is a living artifact — end by telling the user to re-run this when their offer or platform mix changes.
- Force exactly one primary goal. Two primary goals means no strategy, just wishes.
- Prefer the creator's real posts over admired-creator samples; imitation is a fallback, not the default.
