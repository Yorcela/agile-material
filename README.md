# Agile Material

Plugin Claude Code regroupant des outils pour les coachs et équipes agiles : diagnostics,
ateliers, rétrospectives, jeux, formation, etc.

## Structure du plugin

```
.claude-plugin/
  plugin.json          # manifeste du plugin
skills/
  choix-framework-agile/
    SKILL.md           # questionnaire de découverte -> recommandation de framework
agents/                # (à venir) agents spécialisés, ex: coach agile conversationnel
commands/              # (à venir) commandes courtes, ex: /retro, /planning-poker
```

Chaque nouvel outil agile s'ajoute comme un skill (`skills/<nom>/SKILL.md`) ou un agent
(`agents/<nom>.md`) indépendant, avec sa propre description de déclenchement.

## Skills disponibles

- **choix-framework-agile** : à travers une série de questions sur le contexte, les
  ressources/culture et les ambitions de l'organisation, aide à déterminer le framework
  agile le plus pertinent (Scrum, Kanban, SAFe, LeSS, Shape Up...).

## Roadmap (idées à développer)

- Rétrospectives : formats guidés (Start/Stop/Continue, Mad Sad Glad, 4L...) + facilitation.
- Jeux agiles : catalogue de jeux (planning poker, estimation, ice breakers) avec règles.
- Coaching : diagnostics d'équipe, détection d'anti-patterns, plans de progression.
- Formation : supports pédagogiques pour introduire Scrum/Kanban/SAFe à une équipe.
