---
name: rewrite-rules
description: Layer-by-layer content transformation rules for the live fix
---

# Rewrite Rules

Apply these transformations to the lowest-scoring content piece. Work layer by layer — each layer builds on the previous.

## Layer 1 Fix: Vocabulary

**Find and replace:**
- Every forbidden phrase → delete or replace with a specific claim
- "Game-changing" → [delete, or replace with the specific change: "cuts publishing time from 6 hours to 20 minutes"]
- "Leverage" → use the actual verb: "use," "apply," "run," "connect"
- "Proven methodology" → name the methodology or cite the proof: "a 5-layer guardrail system tested across 11 brands"
- "Drive results" → name the results: "generate 3x more qualified pipeline conversations"
- "We're passionate about" → delete entirely. Show passion through specificity, not declaration.

**Soft warning upgrades:**
- "Innovative" → describe what's actually new: "the first system that enforces brand voice through code, not guidelines"
- "Seamless" → describe the experience: "syncs in under 3 seconds with zero manual mapping"
- "Comprehensive" → list what's included: "covers voice, vocabulary, structure, tone, and proof density"

**Rule:** If you can't substantiate it, cut it. Shorter + specific beats longer + vague.

## Layer 2 Fix: Structure

**Add missing structural elements in this order:**

1. **Buyer context** (if missing): Open with the buyer's world, not your solution.
   - Before: "Our AI-powered platform transforms content creation."
   - After: "If you're a founder spending 6+ hours a week on content that isn't generating pipeline..."

2. **Problem specificity** (if generic): Replace abstract pain with concrete scenario.
   - Before: "Most founders struggle with content."
   - After: "Your last 10 LinkedIn posts averaged 12 impressions because they sound identical to every other SaaS founder in your space."

3. **Stakes** (if missing): Name what's at risk.
   - Before: [nothing]
   - After: "Every week without differentiated content is a week your competitors are building the authority you're not."

4. **Evidence** (if missing): Insert at least one proof element.
   - Before: "We help founders create better content."
   - After: "In 30 days, we built a system for a $2M SaaS founder that took content production from 6 hours/week to zero — fully automated, fully on-brand."

5. **Action** (if generic): Replace "let's connect" with a specific next step.
   - Before: "DM me to learn more."
   - After: "Reply with your website URL and I'll show you the 3 biggest gaps in your content system."

## Layer 3 Fix: Proof Density

**For every claim without adjacent proof:**
- Option A: Add a proof element (metric, time frame, named outcome, mechanism)
- Option B: Delete the claim — it's dead weight without proof
- Option C: Soften the claim to match available evidence

**Proof insertion formula:**
```
[Claim] — [proof type]: [specific evidence]
```

Example:
- Claim: "Our system improves content quality."
- Fixed: "Our guardrail system caught 23 vocabulary violations and 4 structural gaps in a single blog post — the kind of drift that accumulates when you're publishing without a system."

**Target:** Every paragraph should have at least one proof element. If a paragraph is 100% claims, either add proof or merge it into an adjacent paragraph that has proof.

## Layer 4 Fix: Voice Consistency

**Using the voice profile from voice-analysis.md:**

- Match authority level: If site is level 3 (confident), don't write at level 5 (absolute) or level 1 (tentative)
- Match formality: If site uses contractions and "you," the rewrite should too
- Match emotional temperature: If site is warm-professional (2-3), don't write hype (5) or clinical (1)
- Weave in differentiator: The thing they said in Q2 should appear naturally in the rewrite, not as a bolted-on tagline
- Use their vocabulary: If the site says "consulting engagements" not "projects," use "consulting engagements"

**Anti-pattern:** Don't overcorrect into a robotic brand voice. The goal is recognizable consistency, not a style straitjacket.

## Layer 5 Fix: Buyer Alignment

**Flip the perspective:**

- Count "we/our/us" sentences. For each one, ask: can this be rewritten from the buyer's perspective?
  - Before: "We built a system that automates content production."
  - After: "You stop spending 6 hours a week on content. The system handles production — you just approve."

- Replace feature language with outcome language:
  - Before: "Our platform includes AI-powered voice analysis."
  - After: "Every piece of content sounds like you wrote it, because the system learned your voice from 50+ samples."

- Make the buyer's role explicit:
  - Before: "Content infrastructure for growing companies."
  - After: "If you're a founder doing $1-5M and you're still the bottleneck for every blog post, social update, and email..."

**Test:** Read the rewritten piece and ask: "If I removed the company name, would I know who this is for?" If yes, buyer alignment is working.

## Output Format for the Rewrite

Present as a before/after with per-layer scores. See templates/audit-report.md for exact formatting.

## Context

This is a reference file for the "whystrohm-audit" Claude Code skill. Claude reads this during Phase 2 (the live fix) to systematically rewrite the lowest-scoring content piece.
