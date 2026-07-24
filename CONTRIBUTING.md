# Contributing to Awesome Marketing Skills

Thank you for helping marketers get real work done with LLM agents. This list stays useful because it is **selective**: every entry has a canonical source, a clear marketing use case, and an honest note about portability and side effects.

## What we accept

A strong entry meets all of these:

- **Canonical source.** Link the original project, not a fork, mirror, or repost.
- **Real marketing use case.** It helps someone do strategy, copy, SEO, content, campaigns, social, analytics, or distribution work — not just "prompts about marketing."
- **Documented format and hosts.** The project says what it is (Agent Skill, Claude plugin, MCP connector, CLI, script bundle) and where it runs (Claude, ChatGPT/Codex, Manus, Cursor, etc.).
- **Disclosed side effects.** Scripts, credentials, API keys, telemetry, MCP connections, sending, publishing, or CRM writes are called out — by the project or by your entry's review note.
- **Active and reachable.** The repository exists, is public, and is not abandoned or archived without notice.

## What we do not accept

- Generic prompt collections with no skill packaging or workflow.
- Cloned duplicates of projects already listed.
- Paywalled tools without a meaningful skill layer.
- Anything that encourages spam, fake engagement, deceptive reviews, deliverability abuse, or unauthorized scraping.
- Entries written primarily to promote a product rather than to describe a working skill.

## How to add an entry

1. Fork this repository and create a focused branch, such as `add-social-analytics-skill`.
2. Add the entry to the most relevant table in `README.md`. Keep the four-column structure used by that table and keep the description concise and factual.
3. Add a numeric reference in the **References** section at the bottom of `README.md`, continuing the existing numbering.
4. Add or update a row in [`catalog-validation.csv`](catalog-validation.csv) so reviewers can audit the selection.
5. Run `git diff --check`, verify every link resolves, and open a pull request using the repository template.
6. In the pull request description, state whether you personally tested the skill, on which host, and whether it read data, wrote data, sent messages, published content, used paid APIs, or required credentials.

## Style guide

- Sentence case for descriptions; no marketing superlatives ("best", "ultimate", "game-changing").
- Describe what the skill *does*, not what its README promises.
- One entry per row; alphabetical order is not required — tables are ordered by usefulness to a newcomer.
- Keep review notes specific: "installer pipes remote shell script" beats "be careful."
- US English, Oxford spelling not required.

## Reporting problems

- **Unsafe installer or undisclosed side effect:** open an issue immediately — these are prioritized over new entries.
- **Stale link or dead project:** open an issue or a small PR removing/annotating the entry.
- **Compatibility claim that no longer holds:** open a PR correcting the entry with a link to the current upstream documentation.

Small documentation fixes and safety corrections are especially welcome and are usually merged fast.

## Review process

Maintainers check the canonical source, skim the skill package (including scripts and installers), and verify the side-effect disclosure before merging. Entries with undisclosed write-capable integrations are sent back for revision, not merged with a warning added later.

## License

By contributing you agree that your contributions are licensed under the [MIT License](LICENSE).
