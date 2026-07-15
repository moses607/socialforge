---
name: visual-idea-generator
description: Turns a post idea into copy-paste text-to-image PROMPTS plus layout briefs for thumbnails, carousels, and Reel/Short covers. Produces a concept, the exact on-image text, and a paste-ready generation prompt (style + aspect ratio) per asset for any image tool (Midjourney, DALL·E, Ideogram, Adobe Firefly, Canva). It writes briefs and prompts only — it does not render images itself. Use when the user asks "what should the image be", needs a thumbnail, carousel, cover, or design brief, or wants visuals that stop the scroll. Trigger on thumbnail, carousel, cover, visual, design brief. Works with any capable model.
---

# Visual Idea Generator

A visual has ~0.4 seconds to win the scroll, so it must communicate ONE idea pre-read: a single subject, one emotion, one promise. Attention is won by contrast and curiosity, not detail — the eye locks onto a human face showing emotion, then reads at most 3 words, then decides. Design from the thumbnail backwards: pick the emotional beat first, compose for a 120px-wide phone preview, and only then write the generation prompt. This skill outputs briefs and prompts you paste into an image tool; it never claims to render pixels itself.

## 1. Thumbnail psychology (the 5 laws)
1. **One subject, one focal point.** A face, an object, or a before/after — never all three. If you can't name the subject in one word, cut.
2. **Emotion on a face beats everything.** Wide eyes, open mouth, genuine shock/joy. Faces looking AT the viewer or AT the object of interest. This is the single biggest CTR lever.
3. **Contrast is king.** Subject must pop off the background: rim light, blurred/darkened backdrop, or complementary color behind the subject (orange subject on teal, yellow on navy). Avoid busy backgrounds.
4. **≤3 words of on-image text**, 1 short line, huge and bold (readable at 120px). Text and face must not overlap. Use a punchy word ("WRONG", "$0 → $10K", "DON'T").
5. **Curiosity gap, not spoiler.** Show the stakes, hide the payoff. "I tried it for 30 days" + a shocked face beats "It grew 4x." Open a loop the title/caption closes.

## 2. Carousel architecture (the 3-act build)
1. **Cover slide = the hook.** Big claim or number + a visual promise of value. Add "swipe" affordance (arrow, "1/7", cut-off next slide). This slide alone decides swipe-through — spend 50% of effort here.
2. **Value slides (3–8).** One idea per slide, consistent template (same margins, font, accent color). Number them. Front-load the best 2 tips — most drop-off happens by slide 3. Use tension → resolution per slide.
3. **CTA slide.** Recap in one line, then ONE ask: follow, save, comment a keyword, or "share this." Never stack CTAs. Restate the handle.

## 3. From concept to prompt
1. Name the emotional beat and the single subject.
2. Write the on-image text (≤3 words, or per-slide headers).
3. Compose the generation prompt: `[subject] + [emotion/action] + [composition/shot] + [lighting] + [color/contrast] + [style] + [negative: no text if you'll add text yourself] + [aspect ratio]`.
4. Specify aspect ratio explicitly: 16:9 thumbnails, 1:1 or 4:5 carousels, 9:16 Reel/Short covers.

## Output template
```
ASSET: <thumbnail | carousel | reel cover>
CONCEPT: <one-line visual idea + emotional beat>
ON-IMAGE TEXT: "<≤3 words>"   (font: bold condensed sans; placement: <e.g. lower-left>)
GEN PROMPT (paste into image tool):
"<subject>, <emotion/action>, <shot & composition>, <lighting>, <color/contrast>,
<style keywords>, high detail, --ar <16:9|1:1|4:5|9:16>, negative: cluttered background, watermark, distorted hands, extra text"
NOTES: add the on-image text yourself in Canva/editor for crisp, legible type.

— CAROUSEL (repeat per slide) —
SLIDE 1 (COVER): headline "<hook>" | gen prompt "<...>" | swipe cue: "1/N + arrow"
SLIDE n (VALUE): header "<idea>" | gen prompt "<...>"
FINAL (CTA): line "<recap>" | ask "<one CTA>" | handle "@..."
```

## Platform variants
- **YouTube:** 16:9, face + 2–3 words, extreme contrast; design for the small grid preview.
- **Instagram/LinkedIn carousel:** 4:5 (max feed height) or 1:1; consistent template, numbered, save-worthy.
- **TikTok/Reels/Shorts cover:** 9:16; keep text out of the top ~15% and bottom ~20% (UI overlaps); bold text that reads muted/autoplay.
- **Pinterest:** 2:3 vertical, text overlay describing the payoff, keyword-rich.

## Rules
- Design the thumbnail before the content — if you can't make a compelling cover, the idea is weak.
- One subject, one emotion, ≤3 words. Kill anything that competes for the focal point.
- Generate the image WITHOUT baked-in text when legibility matters; add text in an editor for crisp type.
- Always specify aspect ratio and a negative prompt (watermark, cluttered background, distorted hands).
- Curiosity over completeness: open a loop the title/caption closes; never spoil the payoff.
- Never claim to render images — hand over the prompt and brief for the user's image tool.
