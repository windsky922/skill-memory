---
name: project-memory
description: Use when starting, continuing, finishing, reviewing, or summarizing project work in this repository; also use for Chinese requests such as 项目经验, 项目复盘, 记住这个项目, 更新记忆, 继续上次任务, 总结经验, or 让 Codex 学习项目经验. Maintains `.memory-bank/` so Codex can reuse project state, decisions, conventions, and lessons across sessions.
---

# Project Memory

Use this skill to keep durable project knowledge in `.memory-bank/`.

## When To Use

- Starting or resuming work in this repository.
- Completing a meaningful task, milestone, document, analysis, or slide deck.
- The user asks to remember project experience, summarize lessons, continue prior work, or update memory.
- You discover durable project facts, decisions, conventions, recurring mistakes, or workflow preferences.

## Memory Files

- `.memory-bank/status.md`: current project state, active work, next steps.
- `.memory-bank/progress.md`: chronological work log.
- `.memory-bank/lessons.md`: reusable mistakes, patterns, and project experience.
- `.memory-bank/decisions.md`: decisions and their consequences.
- `.memory-bank/architecture.md`: workspace map, structure, and important technical context.
- `.memory-bank/conventions.md`: user preferences, file handling rules, verification norms.
- `.memory-bank/final-retrospective.md`: end-of-project or milestone retrospective.

## Workflow

1. Before meaningful work, read the smallest set of memory files needed for the task.
2. During work, rely on memory as project context, not as a substitute for inspecting current files.
3. After meaningful work, update only the files that changed in substance.
4. Keep entries concise and dated.
5. Store durable conclusions, not raw command output or long chat transcripts.

## Completion Update Rules

- Append completed work and next steps to `progress.md`.
- Update `status.md` when active focus, blockers, or next actions change.
- Add to `lessons.md` only when the lesson should influence future work.
- Add to `decisions.md` when a choice affects future implementation or workflow.
- Update `final-retrospective.md` when a project, milestone, paper, report, dataset analysis, or PPT deliverable is completed.

## Safety

- Do not store secrets, tokens, credentials, private account details, or unnecessary raw sensitive data.
- If a fact is uncertain, mark it as uncertain instead of presenting it as settled.
- Do not overwrite user-authored memory entries without preserving their intent.

