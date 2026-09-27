# Agile Material

A Claude Code plugin gathering tools for agile coaches and teams: diagnostics,
workshops, retrospectives, games, training, and more.

## Plugin structure

```
.claude-plugin/
  plugin.json          # plugin manifest
skills/
  agile-framework-selector/
    SKILL.md           # discovery questionnaire -> framework recommendation
agents/                # (coming soon) specialized agents, e.g. a conversational agile coach
commands/              # (coming soon) short commands, e.g. /retro, /planning-poker
```

Each new agile tool is added as an independent skill (`skills/<name>/SKILL.md`) or agent
(`agents/<name>.md`), with its own trigger description.

## Available skills

- **agile-framework-selector**: through a series of questions about an organization's
  context, resources/culture, and ambitions, helps determine the most relevant agile
  framework (Scrum, Kanban, SAFe, LeSS, Shape Up...).

## Roadmap (ideas to develop)

- Retrospectives: guided formats (Start/Stop/Continue, Mad Sad Glad, 4L...) + facilitation.
- Agile games: catalog of games (planning poker, estimation, icebreakers) with rules.
- Coaching: team diagnostics, anti-pattern detection, progression plans.
- Training: teaching materials to introduce Scrum/Kanban/SAFe to a team.
