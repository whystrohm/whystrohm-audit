# WhyStrohm Content Infrastructure Audit

**A free Claude Code skill that scores your content against the same 5-layer framework used to build content infrastructure for founder-led companies.**

Your content gets a score out of 50. You see exactly what's broken and why. Then one piece gets rewritten live — layer by layer — so you experience the difference, not just read about it.

---

## How It Works

| Phase | What Happens |
|-------|-------------|
| **1. Scrape** | Pulls your website to analyze voice, positioning, and content patterns |
| **2. Profile** | Asks 3 targeted questions about your buyer, differentiator, and content |
| **3. Score** | Rates your content against 5 layers (each 1-10, total out of 50) |
| **4. Diagnose** | Shows exact quotes from your content with specific problems identified |
| **5. Rewrite** | Rewrites your lowest-scoring piece live with before/after comparison |
| **6. Reveal** | Explains the full 5-layer framework so you understand the system |

## The 5 Layers

| Layer | What It Checks |
|-------|---------------|
| **Vocabulary** | Hype words, hollow verbs, vendor-centric language, proof density |
| **Structure** | Buyer context, problem specificity, stakes, evidence, clear action |
| **Proof Density** | Claims-to-evidence ratio — every assertion needs adjacent proof |
| **Voice Consistency** | Does your content match your actual brand, or a generic template? |
| **Buyer Alignment** | Written FOR your buyer, or talking about yourself? |

---

## Install

**One command:**

```bash
git clone https://github.com/whystrohm/whystrohm-audit.git ~/.claude/skills/whystrohm-audit
```

**Or manually:** Download this repo and copy the `whystrohm-audit/` folder to `~/.claude/skills/`.

### Requirements

- [Claude Code](https://claude.ai/code) (CLI, desktop app, or IDE extension)
- No API keys. No external tools. No configuration.

---

## Run

```
/whystrohm-audit
```

You'll be asked for:
1. Your website URL
2. Your ideal buyer (role, size, industry)
3. Your differentiator (what you do differently)
4. One piece of published content (LinkedIn post, email, blog paragraph — anything)

The audit takes about 2 minutes.

---

## What You'll See

```
═══════════════════════════════════════
  YOUR CONTENT INFRASTRUCTURE SCORE
═══════════════════════════════════════

                 27/50

  Vocabulary:       7/10  ███████░░░
  Structure:        4/10  ████░░░░░░
  Proof Density:    3/10  ███░░░░░░░
  Voice Consistency:7/10  ███████░░░
  Buyer Alignment:  6/10  ██████░░░░

═══════════════════════════════════════
```

Followed by:
- Per-layer breakdown with **exact quotes** from your content
- Your top 3 content gaps ranked by business impact
- A live rewrite of your weakest piece with before/after scores
- The complete 5-layer framework explained

---

## File Structure

```
whystrohm-audit/
├── SKILL.md                  # Orchestrator — controls the two-phase flow
├── rules/
│   ├── scoring-rubric.md     # The 5-layer framework with scoring criteria
│   ├── voice-analysis.md     # How brand voice is inferred from your website
│   └── rewrite-rules.md      # Layer-by-layer transformation rules
├── templates/
│   ├── audit-report.md       # Output formatting (score display, breakdowns)
│   └── cta.md                # Closing pitch (configurable booking link)
├── LICENSE
└── README.md
```

---

## Want the Full System?

This skill scores 1 piece of content in 2 minutes.

A full content infrastructure install scores your **entire library**, maps voice drift across all platforms, builds the guardrails as code, and hands you a system that produces brand-consistent content without routing everything through the founder.

**What the full system includes:**
- Brand voice encoded as 40-60 enforceable rules (not a PDF)
- Content guardrails that reject hype and require proof before publish
- Video production pipeline (Remotion + FFmpeg + TTS)
- Multi-platform posting automation
- Templates, calendars, and a content engine your team owns completely

**30-day build. You own everything. No retainer. No lock-in.**

Book your content infrastructure diagnostic — 30 minutes, no pitch, just more of what you experienced here:

**https://whystrohm.com/audit**

---

## About WhyStrohm

[WhyStrohm](https://whystrohm.com) builds content infrastructure for founder-led companies doing $500K-$5M. One person. 10+ years in defense systems engineering. No templates. No outsourcing. Systems that run your brand — built and handed over.

## License

MIT — see [LICENSE](LICENSE).
