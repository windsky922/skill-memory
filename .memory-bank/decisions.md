# Decisions

Record project-level decisions that should guide future work.

## Format

```text
YYYY-MM-DD - Decision title
- Decision:
- Reason:
- Consequence:
```

## Entries

- 2026-04-27 - Use Codex-native project memory
- Decision: Store project experience in `.memory-bank/` and expose the workflow through `.agents/skills/project-memory/`.
- Reason: Codex reads repo skills and project instructions directly, which matches this development environment.
- Consequence: Future sessions can recover project state by reading local memory files instead of relying only on chat history.

