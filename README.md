# VersusF VSCode Github Copilot Customization

A public collection of GitHub Copilot custom agents and prompt utilities for practical daily workflows.

This repository starts with one production-ready agent focused on pre-PR review.
Over time, more utilities will be added for analysis, automation, and quality checks.

## Why this repository

Most AI setups are generic. This repo focuses on opinionated, reusable workflows that are:

- Fast to run in real projects
- Easy to adapt to personal/team conventions
- Transparent in behavior and review criteria
- Versioned like code, so improvements are trackable

## Current status

- 1 custom agent available
- Repository structure already prepared for multi-agent growth
- GPL-3.0 license

## Repository structure

agents/pr-review.agent.md

## Available agents

### PR Reviewer

**Purpose**: pre-PR review before opening a pull request

**Main flow**: compare current branch against develop, inspect commits and changed files, report issues by severity

**Output style**: actionable findings with clear verdict (ready, minor changes, blocking)

## Quick start

1. Clone this repository.
2. Copy the desired agent file from the agents folder into your VS Code user prompts location.
3. Open Copilot Chat in Agent mode.
4. Select the PR Reviewer agent.
5. Run the review on your working branch.

## Recommended usage:

- Provide ticket/story context when available
- Run before opening PR
- Address blocking and warning findings before team review

## Design principles

Review what changed, not unrelated legacy code
Prioritize correctness and security first
Keep findings concrete, reproducible, and fix-oriented
Avoid noisy feedback and generic commentary
Prefer deterministic steps over vague reasoning

## Contributing

Contributions are welcome.

Please open an issue or pull request with:

- Use case and expected behavior
- Why existing agents are not sufficient
- Proposed agent or prompt design
- Example input/output if possible

Contribution expectations:

- Keep instructions explicit and testable
- Use clear severity and verdict semantics
- Avoid project-specific secrets or internal-only assumptions
- Keep wording concise and implementation-oriented

## License

GPL-3.0
