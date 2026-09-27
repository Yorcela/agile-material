---
name: choix-framework-agile
description: Aide un utilisateur à choisir le framework agile (Scrum, Kanban, SAFe, LeSS, Shape Up, Spotify Model, etc.) le plus adapté à son organisation, via un questionnaire de découverte sur son contexte, ses ressources/culture et ses ambitions. À utiliser quand l'utilisateur veut démarrer une démarche agile, changer de framework, ou ne sait pas quel cadre choisir pour son équipe/organisation.
---

# Choix du framework agile

Ce skill guide un diagnostic conversationnel pour recommander le framework agile le plus
pertinent pour une organisation donnée. Il ne s'agit pas de plaquer un cadre théorique,
mais de partir du contexte réel de l'utilisateur pour arriver à une recommandation
argumentée, avec ses compromis assumés.

## Comment conduire l'entretien

- Pose les questions **par petits groupes** (2-4 à la fois), pas toutes d'un coup : c'est
  une conversation, pas un formulaire.
- Adapte les questions suivantes au contexte déjà connu (ne repose pas une question dont
  la réponse est évidente ou déjà donnée).
- Reformule brièvement ce que tu as comris avant d'enchaîner, pour valider ta compréhension.
- Si l'utilisateur ne connaît pas la réponse à une question (ex: nombre d'équipes), aide-le
  à l'estimer plutôt que de bloquer dessus.
- Une fois assez d'informations réunies (voir "Quand s'arrêter" plus bas), passe à la
  synthèse et à la recommandation.

## Les 4 dimensions à explorer

### 1. Contexte organisationnel
- Quelle est la taille de l'organisation concernée (nombre de personnes dans les équipes
  produit/tech) ?
- Combien d'équipes sont concernées par la démarche ? Une seule équipe, plusieurs équipes
  travaillant sur un même produit, ou plusieurs équipes/produits indépendants ?
- Quel type de produit/activité (logiciel produit, projet client, plateforme interne,
  matériel/hardware, secteur réglementé...) ?
- Y a-t-il des dépendances fortes entre équipes, ou peuvent-elles travailler de façon
  largement autonome ?
- Où en est l'organisation aujourd'hui : aucune pratique agile, agile informel ("agile de
  façade"), ou une transformation déjà engagée avec un framework existant ?

### 2. Ressources et culture
- Quel est le niveau de maturité agile des équipes et du management (débutant,
  intermédiaire, expérimenté) ?
- Le management est-il prêt à déléguer des décisions aux équipes, ou la culture reste-t-elle
  très hiérarchique/command-and-control ?
- Y a-t-il un budget et un temps dédiés pour de la formation/du coaching, ou faut-il un
  cadre qui s'apprend "sur le tas" ?
- Le rythme de travail est-il plutôt orienté flux continu (support, exploitation,
  maintenance) ou plutôt orienté livraisons/itérations cadencées (nouveaux produits,
  fonctionnalités) ?
- Y a-t-il des contraintes fortes de prévisibilité/reporting (engagements clients,
  comité de direction, contractuel) ?

### 3. Contraintes
- Y a-t-il des contraintes réglementaires ou de conformité (santé, finance, aéronautique...)
  qui imposent traçabilité, documentation, validations ?
- Le time-to-market est-il critique, ou la qualité/stabilité prime-t-elle sur la vitesse ?
- Y a-t-il des contraintes de synchronisation avec d'autres entités (portefeuille de
  projets, autres départements, partenaires externes) ?
- Quel est l'horizon de la démarche : test sur une équipe pilote, ou déploiement à l'échelle
  dès le départ ?

### 4. Ambitions
- Qu'est-ce qui motive la démarche : améliorer la livraison de valeur, réduire les délais,
  améliorer la qualité, améliorer l'engagement des équipes, préparer une mise à l'échelle ?
- L'ambition est-elle de faire évoluer une seule équipe, ou de structurer l'agilité à
  l'échelle de plusieurs équipes/départements à moyen terme ?
- Y a-t-il une préférence culturelle déjà exprimée (ex: "on ne veut pas de rôles figés",
  "on veut un cadre très simple", "on veut un cadre qui a fait ses preuves à grande
  échelle") ?

## Quand s'arrêter

Tu as assez d'informations dès que tu peux répondre à ces 4 questions :
1. Combien d'équipes, et sont-elles interdépendantes ?
2. Flux continu ou itératif ?
3. Culture : hiérarchique/directive ou autonome/collaborative, et niveau de maturité agile ?
4. Contrainte dominante : prévisibilité/conformité, vitesse, ou qualité/engagement ?

Si l'utilisateur veut aller vite, tu peux poser ces 4 questions directement au lieu du
détail ci-dessus.

## Grille de décision

Utilise cette grille comme guide de raisonnement, pas comme un algorithme rigide : le but
est d'arriver à **une recommandation principale + une alternative**, avec la justification
qui relie les réponses de l'utilisateur au choix.

| Signal dominant | Framework(s) à considérer en priorité |
|---|---|
| Une seule équipe, produit avec un backlog clair, rythme itératif souhaité, ambition d'installer une cadence régulière | **Scrum** |
| Flux de travail continu, forte proportion de demandes non planifiables (support, exploitation, maintenance), peu d'appétence pour des rôles/cérémonies formels | **Kanban** |
| Une seule équipe mais culture très allergique aux rôles/process figés, besoin de flexibilité maximale, produit en phase d'exploration | **Kanban**, ou **Scrum allégé** |
| Plusieurs équipes (2 à ~5) sur un même produit, forte dépendance entre elles, besoin de synchronisation sans lourdeur | **LeSS** (si petite échelle) ou **Scrum of Scrums / Nexus** |
| Mise à l'échelle sur de nombreuses équipes, contraintes de prévisibilité fortes (engagements, portefeuille, budget), organisation plutôt hiérarchique habituée à des processus formels | **SAFe** |
| Mise à l'échelle sur plusieurs équipes, culture voulant rester légère et éviter la lourdeur de process, priorité à l'autonomie des équipes | **LeSS** ou **Spotify Model** (à adapter, ce n'est pas un framework figé) |
| Produit avec des cycles de découverte/livraison longs, équipe senior et autonome, volonté d'éviter le détail de planification à l'avance (pas de sprint planning classique) | **Shape Up** |
| Contraintes réglementaires fortes, traçabilité et documentation obligatoires, secteur critique (santé, aéronautique, finance) | **SAFe** ou **Scrum avec adaptations de conformité** (jamais un cadre "pur" qui ignore la contrainte) |
| Organisation en toute première découverte de l'agilité, faible maturité, besoin d'un cadre simple à enseigner | **Scrum** (le plus documenté/outillé pour démarrer), en évitant SAFe à ce stade |

Points de vigilance à mentionner explicitement dans la recommandation :
- **SAFe** est souvent sur-dimensionné pour une organisation qui n'a pas encore expérimenté
  l'agilité à petite échelle : le proposer implique d'alerter sur le risque de lourdeur et de
  recommander un pilote avant généralisation.
- **Shape Up** suppose une équipe autonome et un fort niveau de confiance/maturité ; il est
  rarement adapté à une équipe junior ou à un contexte très directif.
- Le "Spotify Model" n'est pas un framework prescriptif mais une source d'inspiration
  organisationnelle (tribus/squads) : le présenter comme tel, jamais comme une méthode
  clé en main.
- Un cadre hybride (ex: Scrum au niveau équipe + Kanban pour le support, ou Scrum avec un
  allégement des cérémonies) est une réponse légitime si le contexte est mixte : ne pas
  forcer un choix unique si la réalité est hybride.

## Format de la recommandation finale

Termine toujours par une synthèse structurée :

1. **Résumé du contexte** compris (2-3 phrases, pour valider avec l'utilisateur).
2. **Recommandation principale** : le framework, en une phrase claire.
3. **Pourquoi** : 3 à 5 points reliant explicitement les réponses de l'utilisateur au choix
   (pas de justification générique).
4. **Alternative à considérer** : un second framework plus léger ou plus ambitieux, avec la
   condition qui ferait basculer vers lui.
5. **Risques et points de vigilance** : ce qui pourrait faire échouer ce choix dans ce
   contexte précis, et comment l'anticiper.
6. **Premiers pas concrets** : 2-3 actions pour démarrer (ex: "commencer par une équipe
   pilote pendant 2 sprints avant d'étendre", "former les Product Owners avant le
   lancement").

Garde un ton de conseil, pas de verdict définitif : rappelle que le choix peut évoluer une
fois testé, et que l'important est d'itérer sur le framework lui-même comme sur le produit.
