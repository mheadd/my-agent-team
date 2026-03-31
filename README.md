# My Agent Team

A four-agent chain that takes a software specification from planning to pull request. An **Orchestrator** governs the workflow, a **Builder** writes the code, a **Reviewer** evaluates it, and a **Shipper** prepares the PR.

## How It Works

1. Start with the **Orchestrator** — it reviews the spec for ambiguity, declares scope, and drives the process.
2. The **Builder** implements the spec in discrete, committed chunks.
3. The **Reviewer** evaluates the output and returns a PASS or FAIL verdict.
4. The **Shipper** prepares the pull request and updates the changelog.

The chain includes human checkpoints for spec clarification and architectural decisions. See [AGENTS.md](AGENTS.md) for full details on conventions, skills, and agent behavior.
