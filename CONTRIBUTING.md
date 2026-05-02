# Contributing to awesome-statefun

## What to add

- **Runtimes** that implement Apache Stateful Functions or comparable durable-actor models on Apache Flink.
- **SDKs** that target the request-reply HTTP protocol or embedded function model.
- **Examples and playgrounds** with working code that builds.
- **Production guides** with concrete deployment patterns.
- **Related actor frameworks** in adjacent ecosystems (durable execution, virtual actors, workflow engines) — *only if* they're well-documented and broadly used.
- **Articles and talks** that are genuinely instructive — vendor blog posts welcome if they contain technical depth.

## Quality bar

- Project must be **publicly available** (open-source preferred; closed-source allowed if the docs are public and substantial).
- Entry must be **actively useful** — last commit or release within ~24 months unless the project is officially archived but historically significant.
- Entry must include a **one-sentence description** that says what it does, not what it isn't.

## Format

Each entry follows this format:

```markdown
- [Project name](https://link) — One sentence describing what it does. Optional second sentence with the most important constraint or capability.
```

Avoid:

- Marketing language ("best", "fastest", "most powerful")
- Defensive framing ("actively maintained", "production-ready" — let the link speak for itself)
- Keyword stuffing
- Multi-paragraph descriptions

## Submitting a PR

1. Fork this repository
2. Add your entry to the appropriate section, alphabetically
3. Run a quick spell-check / link-check
4. Open a PR with a body that says: *"Adds X to section Y. [Link]. Brief reason it fits."*

PRs that follow these guidelines are typically reviewed within a week.
