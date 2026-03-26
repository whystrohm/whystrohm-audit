---
name: audit-report
description: Output format template for the WhyStrohm content diagnostic
---

# Audit Report Format

Use this exact format for the Phase 1 diagnostic output. Score first, details second.

## Score Display (Show This First)

```
═══════════════════════════════════════
  YOUR CONTENT INFRASTRUCTURE SCORE
═══════════════════════════════════════

                 {score}/50

  Vocabulary:       {v}/10  {v_bar}
  Structure:        {s}/10  {s_bar}
  Proof Density:    {p}/10  {p_bar}
  Voice Consistency:{vc}/10 {vc_bar}
  Buyer Alignment:  {ba}/10 {ba_bar}

═══════════════════════════════════════
```

**Bar format:** Use block characters to visualize each score.
- Full block per point: e.g., 7/10 = `███████░░░`
- Makes the score feel tangible, not just a number.

**Pause here.** Let the score sit for a beat before continuing. Use a line break.

## Layer Breakdown (Show After Score)

For each layer, use this format:

```
### {Layer Name}: {score}/10

**What this means:** [One sentence interpreting the score]

**Evidence from your content:**
- "{exact quote from their content}" — [why this is a problem]
- "{exact quote}" — [specific issue]
- "{exact quote}" — [specific issue]

**What infrastructure-grade looks like:** [One sentence showing the standard]
```

**Rules:**
- Always quote their actual content. Never paraphrase.
- Always explain WHY the quote is a problem, not just that it is one.
- Limit to 3 examples per layer. Pick the worst offenders.
- "Infrastructure-grade" line shows the bar without being preachy.

## Top 3 Issues

After all 5 layers, present:

```
## Your Top 3 Content Gaps

1. **{Most impactful issue}** — {One sentence}. This is costing you {consequence}.
2. **{Second issue}** — {One sentence}. {Consequence}.
3. **{Third issue}** — {One sentence}. {Consequence}.
```

**Rules:**
- Rank by business impact, not by score.
- Consequences should be specific to their buyer and industry.
- Each gap should feel fixable (not hopeless) but systemic (not a quick tweak).

## Framework Explanation

After top 3, transition to the framework reveal:

```
## The System Behind This Score

What you just experienced is a 5-layer content infrastructure audit. Here's what each layer enforces and why it matters:

**1. Vocabulary Control** — Your content is only as strong as its weakest word. Hype language ("game-changing," "leverage," "innovative") signals to sophisticated buyers that there's no substance behind the claim. Vocabulary control enforces proof-dense language by flagging and replacing hollow phrases.

**2. Structural Enforcement** — Great content isn't just well-written — it's well-built. Every piece needs buyer context, problem specificity, stakes, evidence, strategic implications, and a clear action. When these elements are missing, content feels like noise.

**3. Proof Density** — Claims without proof are just opinions. Proof density measures whether every assertion has adjacent evidence — a metric, a time frame, a named outcome, or a mechanism explanation. This is what separates authority from hype.

**4. Voice Consistency** — Your website says one thing. Your content says another. Voice consistency checks whether your content actually sounds like your brand, or like a generic marketing template. Drift here erodes trust.

**5. Buyer Alignment** — The most common failure: content that talks about the company instead of talking to the buyer. Buyer alignment measures whether every paragraph serves the person you're trying to reach, or just describes what you do.

These five layers run on every piece of content, every platform, automatically. Not as guidelines — as code. That's what content infrastructure means.
```

## Before/After Display (Phase 2)

Use this format for the live rewrite comparison:

```
═══════════════════════════════════════
  BEFORE → AFTER
═══════════════════════════════════════

BEFORE ({before_score}/50)
───────────────────────────
{original content}

  Vocabulary:       {v}/10
  Structure:        {s}/10
  Proof Density:    {p}/10
  Voice Consistency:{vc}/10
  Buyer Alignment:  {ba}/10

AFTER ({after_score}/50)
────────────────────────
{rewritten content}

  Vocabulary:       {v}/10  (+{diff})
  Structure:        {s}/10  (+{diff})
  Proof Density:    {p}/10  (+{diff})
  Voice Consistency:{vc}/10 (+{diff})
  Buyer Alignment:  {ba}/10 (+{diff})

═══════════════════════════════════════
```

**Show the delta** on each layer so they see exactly where improvement happened.
