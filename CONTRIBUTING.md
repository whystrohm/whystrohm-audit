# Contributing to WhyStrohm Audit

Thanks for your interest in improving this skill.

## Reporting Issues

If the skill produces unexpected output, misscores content, or breaks during the flow:

1. Open an [issue](https://github.com/whystrohm/whystrohm-audit/issues/new?template=bug_report.md)
2. Include:
   - Your Claude Code version (`claude --version`)
   - What step of the audit broke or behaved unexpectedly
   - What you expected vs. what happened
   - The content you were auditing (or a sanitized version)

## Suggesting Improvements

Ideas for new scoring layers, better rubric criteria, or flow improvements:

1. Open an [issue](https://github.com/whystrohm/whystrohm-audit/issues/new?template=feature_request.md) describing the change
2. Explain why it improves the audit for the end user
3. If proposing a scoring change, include a before/after example

## Pull Requests

1. Fork the repo
2. Create a branch (`git checkout -b improve-scoring-rubric`)
3. Make your changes
4. Test by running `/whystrohm-audit` in a fresh Claude Code session
5. Submit a PR with a clear description of what changed and why

## Code of Conduct

See [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md).

## Questions?

This skill is maintained by [WhyStrohm](https://whystrohm.com). For questions about the methodology or the full content infrastructure service, visit https://whystrohm.com/audit.
