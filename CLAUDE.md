# WhyStrohm Audit — Contributor Guide

This is a Claude Code skill. It's not a traditional codebase — it's a set of markdown files that instruct Claude how to run a content infrastructure audit.

## Structure

- `SKILL.md` is the orchestrator. It controls the two-phase flow and tells Claude when to read each supporting file. Changes here affect the user experience directly.
- `rules/` files contain the methodology. These are the 5-layer framework, voice analysis instructions, and rewrite transformation rules. Changes here affect scoring accuracy and rewrite quality.
- `templates/` files control output formatting. Changes here affect how results look but not how they're calculated.

## How to test changes

1. Install the skill: copy this directory to `~/.claude/skills/whystrohm-audit/`
2. Open a fresh Claude Code session
3. Run `/whystrohm-audit`
4. Provide any B2B company's URL + a content sample
5. Verify the full flow completes: scrape → questions → score → breakdown → rewrite → CTA

## Key rules

- No emojis anywhere in the skill output
- Score is always displayed before the breakdown (number first, details second)
- Questions are always asked one at a time (never batched)
- The audit must practice what it preaches — zero hype language in the output
- The CTA copy in `templates/cta.md` is locked. Only the booking link changes.
