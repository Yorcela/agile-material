# Agile Material — design system

Agile Material is the shared visual language for every artifact produced by the plugin of
the same name: kanban boards, retrospectives, roadmaps, sprint reports, demo slides, team
dashboards. It's warm and playful — a well-organized wall of sticky notes — without ever
sacrificing readability: an artifact should work equally well projected in a meeting or
printed out.

## Principles

1. **Warm, not childish.** Rounded shapes, a paper-like background, bold colors — but a
   single identity color (`pine`) and vivid colors reserved for a precise meaning.
2. **Color has meaning.** `pine` = done / primary action, `sun` = in progress / idea,
   `coral` = blocked / risk, `sky` = to do / info. A single artifact never repurposes
   these roles.
3. **Content first.** Titles in Fredoka set the tone; everything else is in Nunito, at a
   readable size (16px minimum for body text).
4. **Cards, not rows.** The base unit is the card / sticky note: `surface-raised`,
   `radius-md`, `shadow-sm`, `space-4` padding.

## Voice and content

- Tone can be formal or informal depending on the team, but sentences stay short, verbs
  are active, and vocabulary is standard agile vocabulary (sprint, story, backlog, retro,
  velocity).
- Titles use sentence case ("Sprint goals", not "Sprint Goals").
- Labels (`caption`) are uppercase: `TO DO`, `IN PROGRESS`, `BLOCKED`, `DONE`.
- No emoji in titles or data; color and shape already carry the playfulness.
- Numbers and identifiers (`US-142`, `21 pts`) use `code` styling when they need to align.

## Visual foundations

**Colors.** Two themes, Light and Dark, both verified at a 4.5:1 minimum contrast ratio
for text. The page background is `surface`; cards are `surface-raised`; recessed areas
(kanban column, code block) are `surface-sunken`. Text is `ink`, secondary text is
`ink-muted`. Each state color exists in three versions: the solid fill (`pine`, `sun`,
`coral`, `sky`), a soft tint (`*-soft`) for badge and callout backgrounds, and the color
of text placed on the solid fill (`on-*`). `sun` yellow is never used as text on a light
background: use `sun-text` instead.

| Status | Badge (background / text) | Solid (background / text) |
| --- | --- | --- |
| To do | `sky-soft` / `sky` | `sky` / `surface` |
| In progress | `sun-soft` / `sun-text` | `sun` / `on-sun` |
| Blocked | `coral-soft` / `coral` | `coral` / `on-coral` |
| Done | `pine-soft` / `pine` | `pine` / `on-pine` |

**Typography.** `display` (40px) once per artifact; `title` and `heading` to structure
content; `body` for running text; `small` in cards and dense tables; `caption` for
labels. Google Fonts: Fredoka (600, 500), Nunito (400, 700), JetBrains Mono (400).

**Spacing and shapes.** 4px grid (`space-1` through `space-12`). Corners: `radius-sm` for
badges and sticky notes, `radius-md` for buttons and cards, `radius-lg` for columns,
panels and slides, `radius-full` for pills and avatars. Short shadows (`shadow-sm` at
rest, `shadow-lg` for anything floating). Keyboard focus: `focus-ring`.

**Charts.** Series follow the order `pine`, `sky`, `sun`, `coral`; axes and gridlines use
`line`, labels use `ink-muted`. A burndown: actual in `pine`, ideal in dashed
`ink-muted`.

**Avoid.** Gradients, long drop shadows, colored left borders on cards, colors outside
the token set, more than four state colors in a single view.

## Iconography

No icon set or logo yet: the name "Agile Material" is set in Fredoka 600, color `ink`.
In the meantime, use rounded-stroke icons (2px, round caps) in `currentColor`, never
filled with a solid color.
