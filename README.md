# 🚀 SocialForge

**Turn any Claude (or any capable model) into a complete AI social-media growth agency.**

SocialForge is an open-source suite of **20 composable skills** — model-invoked playbooks that encode how top creators actually grow: reverse-engineering competitors, nailing an audience, generating scroll-stopping hooks, writing retention-engineered scripts, turning one video into 30+ posts, riding trends, engineering engagement, and adapting across every platform. An **orchestrator** chains them into end-to-end workflows.

These aren't "act as a social media expert" prompts. Each skill is a repeatable method with an output template, platform variants, and hard rules — the difference between a prompt and a system.

> Works with **Claude** (Opus 4.8, Sonnet 5, Haiku 4.5, Fable 5), Claude Code, Cursor, and any capable model. MIT licensed. Free forever.

---

## ⚡ Install

**Claude Code (recommended):**
```bash
/plugin marketplace add moses607/socialforge
/plugin install socialforge@socialforge
```

**Any agent / API / Claude.ai:** every skill is a self-contained `skills/<name>/SKILL.md`. Upload it as a skill, or paste it as a system/developer instruction. No dependencies.

**Manual:** clone this repo and point your agent's skills directory at `skills/`.

---

## 🧠 The 20 skills

### 🎛️ Orchestration
| Skill | What it does |
|-------|--------------|
| `growth-orchestrator` | Routes a goal to the right skills in the right order and runs them as one workflow |

### 🎯 Foundation & audience
| Skill | What it does |
|-------|--------------|
| `onboarding-brand-brief` | Captures your niche, positioning, goal, and voice into a reusable brief the other skills consume |
| `audience-bullseye` | Hyper-precise persona built on psychographics & jobs-to-be-done — pains, desires, the words they use |
| `channel-competitor-analysis` | Reverse-engineers any creator's hooks, pillars, cadence, and exploitable weaknesses |
| `profile-optimizer` | Turns your profile into a follow-and-convert machine (bio, pinned, link-in-bio) |

### 🔥 Trends & discovery
| Skill | What it does |
|-------|--------------|
| `breakout-detector` | Finds outlier content in your niche before it saturates; scores an idea's breakout potential |
| `trend-jacker` | Rides a trend/sound/news story fast and on-brand — same-day fast lane + cringe check |

### ✍️ Creation
| Skill | What it does |
|-------|--------------|
| `hook-machine` | Generates dozens of scroll-stopping hooks per platform, then cuts to the best 1-3 |
| `viral-script-generator` | Shot-by-shot short-form scripts engineered for retention (hook → beats → payoff → CTA) |
| `content-strategy-engine` | Pillars, content ratios, a format library, and a weekly calendar — a repeatable system |
| `campaign-builder` | End-to-end launch / series / challenge plans with a day-by-day beat sheet |
| `youtube-title-lab` | Generates and stress-tests YouTube title + thumbnail-text pairs for CTR |
| `offer-cta-architect` | Designs the CTA ladder from free content → owned audience → offer, without feeling salesy |

### ♻️ Distribution & consistency
| Skill | What it does |
|-------|--------------|
| `repurpose-master` | Turns one long asset into 30+ short-form pieces, spec'd per platform |
| `cross-platform-adapter` | Adapts one idea to each platform's native norms (not identical cross-posting) |
| `visual-idea-generator` | Paste-ready image prompts + layouts for thumbnails, carousels, and covers |
| `brand-voice-keeper` | Defines and enforces a consistent voice & visual identity with a pass/fail checklist |

### 📈 Community & optimization
| Skill | What it does |
|-------|--------------|
| `engagement-booster` | First-hour tactics, reply strategies, DM flows, and community rituals that drive the signals algorithms reward |
| `analytics-interpreter` | Turns raw metrics into a funnel diagnosis and names the single biggest leak |
| `performance-optimizer` | Post-mortems a piece, proposes A/B tests, and decides kill vs iterate vs scale |

---

## 🎬 Quickstart workflows

Just tell the orchestrator your goal — it picks the chain:

- **"I have one long video, do everything"** → `repurpose-master` → `hook-machine` → `cross-platform-adapter` → `visual-idea-generator`
- **"Grow my new account"** → `onboarding-brand-brief` → `audience-bullseye` → `channel-competitor-analysis` → `content-strategy-engine` → `hook-machine` → `viral-script-generator`
- **"Make this post go viral"** → `channel-competitor-analysis` → `hook-machine` → `viral-script-generator` → `visual-idea-generator`
- **"Why isn't this working?"** → `analytics-interpreter` → `performance-optimizer` → fix the weakest link
- **"Ride this trend now"** → `trend-jacker` → `hook-machine` → `viral-script-generator` (ship same day)

Example:
```
> Use growth-orchestrator: I run a fitness account on Instagram & TikTok, 2k followers,
> and I just recorded a 40-minute podcast. Grow me.
```

---

## 🧩 How skills work

A skill is a directory with a `SKILL.md` (YAML frontmatter + instructions). The model keeps only the one-line description in context and loads the full playbook when your request matches — so you can install all 20 without bloating context. They **compose**: each skill's output feeds the next.

## 🗺️ Roadmap

See [`ROADMAP.md`](ROADMAP.md) — planned: `newsletter-growth`, `ugc-brief`, `comment-mining`, plus platform-specific packs and integration hooks (Make/Zapier/webhooks). Contributions welcome.

## 🤝 Contributing

New skills and improvements are welcome — see [`CONTRIBUTING.md`](CONTRIBUTING.md). Keep the house style: one tight principle, numbered method, an output template, platform variants, and hard rules.

## 💎 Want the pro tiers?

SocialForge is the free growth suite. If you want the deeper, paid packs — production skills for shipping software, meta-skills for operating the model itself, and frontier agent skills — see **[SkillForge](https://github.com/moses607/skillforge)**.

## ⚡ Building agents, not just content?

See **[Aether OS](https://github.com/moses607/aether-os)** — a free, model-agnostic **AI agent kernel** (persistent memory, governed multi-agent orchestrator, eval harness, cost tracking). Apache-2.0. It's the infrastructure these skills run on top of.

## 📄 License

[MIT](LICENSE) © Cherry FRANCOIS. Use it, fork it, ship with it.
