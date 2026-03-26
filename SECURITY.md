# Security Policy

## Reporting a Vulnerability

This is a Claude Code skill — it runs locally in your terminal and does not transmit data to any server. The skill reads your website via public URLs and processes content within your Claude Code session.

If you discover a security concern (e.g., the skill could be manipulated to execute unintended commands, or the scoring rubric contains logic that could be exploited):

**Email:** hello@whystrohm.com

Please include:
- Description of the concern
- Steps to reproduce
- Potential impact

We will respond within 48 hours.

## Scope

This skill has no backend, no database, no authentication, and no network calls beyond WebFetch to URLs you provide. The attack surface is limited to the skill's markdown instructions and how Claude Code interprets them.
