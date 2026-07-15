# Contributing to SocialForge

Thanks for helping build the best open-source social-growth skill suite. Quality over quantity — one sharp skill beats five vague ones.

## Add or improve a skill

1. Create `skills/<kebab-name>/SKILL.md`.
2. Follow the house format exactly:
   ```
   ---
   name: <kebab-name>
   description: <2-4 sentences: what it does + explicit triggers ("Use when...", "Trigger on..."). End with "Works with any capable model.">
   ---

   # <Title>

   <One tight paragraph: the core principle. First-principles, results-oriented. No fluff.>

   ## <2-3 method sections — numbered, concrete steps, real tactics/frameworks/numbers>

   ## Output template
   ` ``
   <a concrete, copy-usable structure the skill produces>
   ` ``

   ## Platform variants
   <short platform-specific notes where relevant>

   ## Rules
   - <5-6 opinionated hard rules>
   ```
3. Add the skill's path to `.claude-plugin/marketplace.json`.
4. Target ~2,800–4,000 characters. Dense and specific beats long and vague.

## The quality bar

- **Provider-agnostic.** Write "the model" / "any capable model", never assume a vendor.
- **Method, not vibes.** Every skill must give a repeatable procedure with an output template someone can act on.
- **Opinionated rules.** The `Rules` section is what separates a pro from an amateur — take a stance.
- **Honest.** Skills that need live data (trends, analytics) must say so and instruct the user to supply it or pair with a browsing/search tool — don't imply real-time knowledge the model doesn't have.
- **No fabricated metrics.** Teach mechanisms; don't promise specific results.

## PRs

Open a PR with the new/changed skill and a one-line rationale. Small, focused PRs merge faster.
