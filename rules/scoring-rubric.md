---
name: scoring-rubric
description: 5-layer content guardrail scoring framework
---

# Content Infrastructure Scoring Rubric

Score each piece of content against these 5 layers. Each layer is 1-10. Total possible: 50.

## Layer 1: Vocabulary (1-10)

**What it checks:** Hype density, hollow verbs, vendor-centric language.

**Forbidden phrases (instant deductions):**
- Hype adjectives: "game-changing," "revolutionary," "world-class," "unparalleled," "best-in-class," "transformative," "cutting-edge," "groundbreaking," "disruptive"
- Hype nouns: "paradigm shift," "magic," "silver bullet," "secret sauce"
- Empty openers: "in today's fast-paced digital landscape," "now more than ever," "take your X to the next level," "the future of X is here," "are you struggling to..."
- Hollow verbs: "leverage," "enable," "optimize," "empower," "unlock," "unleash," "drive impact," "move the needle," "accelerate growth," "maximize ROI"
- Inflated qualifiers: "truly," "really," "deeply," "incredibly," "highly," "significant" (allowed ONLY with adjacent numbers)
- Vendor-centric: "we're passionate about," "we believe in," "our mission is," "we're proud to"

**Soft warnings (deduct if no proof adjacent):**
- "innovative," "seamless," "holistic," "end-to-end," "comprehensive," "robust," "scalable," "strategic partner," "thought leader"

**Scoring:**
- 9-10: Zero forbidden phrases, zero unsubstantiated soft warnings, proof-dense language throughout
- 7-8: Zero forbidden phrases, 1-2 soft warnings with partial substantiation
- 5-6: 1-2 forbidden phrases OR 3+ unsubstantiated soft warnings
- 3-4: 3-5 forbidden phrases, hype-heavy tone
- 1-2: 6+ forbidden phrases, reads like a marketing template

**How to count:** List every flagged word/phrase with its line. Report exact count.

## Layer 2: Structure (1-10)

**What it checks:** Whether the content has the bones of buyer-focused communication.

**Required structural elements:**
- **Buyer context:** Who specifically is this for? (role + seniority + function)
- **Problem specificity:** A concrete situation, not generic pain. "Posting content nobody reads" is generic. "Your Q3 pipeline has 40% fewer qualified leads because prospects can't distinguish you from competitors" is specific.
- **Stakes:** What happens if they don't act? Concrete consequences, not fear mongering.
- **Evidence/Proof:** At least one: metric, time frame, named outcome, mechanism explanation, or case snapshot.
- **Strategic implication:** What this means for their decisions.
- **Action:** Specific next step tied to the buyer's decision — not "let's connect."

**Scoring:**
- 9-10: All 6 elements present and specific
- 7-8: 5 elements present, remaining elements partially addressed
- 5-6: 3-4 elements present
- 3-4: 1-2 elements present, rest missing or generic
- 1-2: No structural elements — stream of consciousness or pure hype

**How to score:** Check each element. Mark present/absent/partial. Count.

## Layer 3: Proof Density (1-10)

**What it checks:** Ratio of claims to evidence. Every strong claim needs adjacent proof.

**Proof types:**
- Metric (number + context): "reduced time-to-publish by 60%"
- Time frame: "in the first 30 days"
- Named outcome: "client went from 2 posts/month to daily publishing"
- Mechanism explanation: "by extracting the founder's voice into a config file that governs all content"
- Case snapshot: "a $2M SaaS founder was spending 6 hours/week on content — now spends zero"

**What counts as a claim:**
- Any result or outcome statement
- Any comparative ("better," "faster," "more effective")
- Any promise about what will happen

**Scoring:**
- 9-10: Every claim has adjacent proof. Proof-to-claim ratio > 1:1.
- 7-8: Most claims supported. 1-2 unsupported but minor.
- 5-6: ~50% claims supported. Pattern of assertion without evidence.
- 3-4: Mostly claims, very little proof. "Trust me" energy.
- 1-2: Pure assertion. Zero proof elements. Content is 100% claims.

**How to count:** List each claim. For each, note whether proof is adjacent (within same paragraph). Calculate ratio.

## Layer 4: Voice Consistency (1-10)

**What it checks:** Whether the content sounds like the brand the person described, or like a generic marketing template.

**Compare against:**
- The voice inferred from their website (see voice-analysis.md)
- The differentiator they stated in Q2
- The buyer they named in Q1

**Signals of inconsistency:**
- Website uses technical language but content is all hype
- Claimed differentiator doesn't appear in the content at all
- Tone shifts between professional and desperate within same piece
- Content could belong to any company in any industry (commodity voice)

**Scoring:**
- 9-10: Content unmistakably belongs to this brand. Differentiator is woven in. Tone matches website.
- 7-8: Mostly consistent. Minor drifts in 1-2 spots.
- 5-6: Partially consistent. Differentiator mentioned but not integrated. Some generic patches.
- 3-4: Mostly generic. Could swap in any company name. Occasional brand signal.
- 1-2: Fully generic. Zero brand fingerprint. Template energy.

## Layer 5: Buyer Alignment (1-10)

**What it checks:** Is this content written FOR the named buyer, or is it the company talking about themselves?

**Signals of misalignment:**
- Sentences start with "We" or "Our" more than "You" or "Your"
- Features described without buyer benefit
- No reference to buyer's daily reality, challenges, or decisions
- CTA is "contact us" (company-centric) vs. "see how this applies to your pipeline" (buyer-centric)
- Content describes what the company does, not what the buyer gets

**Scoring:**
- 9-10: Every paragraph addresses the buyer's world. "You" outnumbers "We" 3:1+. Buyer's role and context are explicit.
- 7-8: Mostly buyer-focused. 1-2 company-centric patches.
- 5-6: Split between buyer and company focus. Reads as half pitch, half value.
- 3-4: Mostly company-focused. Buyer is an afterthought.
- 1-2: Entirely self-referential. "We we we." Buyer is invisible.

**How to count:** Tally "we/our/us" vs "you/your" sentences. Check if buyer role appears.

## Interpreting the Total Score

| Range | Verdict |
|-------|---------|
| 40-50 | Infrastructure-grade. Rare without a system. |
| 30-39 | Solid foundation with specific gaps to close. |
| 20-29 | Common for founder-led brands. Good instincts, no system. |
| 10-19 | Template-driven or outsourced. Voice and buyer disconnected. |
| 1-9 | Content is actively hurting the brand. Needs full rebuild. |

## Context

This is the core methodology file for a Claude Code skill called "whystrohm-audit" — a lead magnet for WhyStrohm's content infrastructure service. The skill audits prospect content against this 5-layer framework, then rewrites one piece live. This file is read by Claude during the scoring phase.
