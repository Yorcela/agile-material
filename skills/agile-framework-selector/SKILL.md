---
name: agile-framework-selector
description: Helps a user choose the agile framework (Scrum, Kanban, SAFe, LeSS, Shape Up, Spotify Model, etc.) best suited to their organization, through a discovery questionnaire covering context, resources/culture, and ambitions. Use when the user wants to start an agile initiative, switch frameworks, or doesn't know which framework to pick for their team/organization.
---

# Agile framework selector

This skill guides a conversational discovery process to recommend the agile framework
most relevant to a given organization. The goal isn't to apply a theoretical template, but
to start from the user's actual context and arrive at a justified recommendation, with its
trade-offs made explicit.

## How to conduct the interview

- Ask questions in **small groups** (2-4 at a time), not all at once: this is a
  conversation, not a form.
- Adapt the questions below to context already known (don't re-ask a question whose
  answer is obvious or already given).
- Briefly rephrase what you understood before moving on, to validate your understanding.
- If the user doesn't know the answer to a question (e.g. number of teams), help them
  estimate rather than getting stuck on it.
- Once enough information has been gathered (see "When to stop" below), move on to the
  summary and recommendation.

## The 4 dimensions to explore

### 1. Organizational context
- What is the size of the organization involved (number of people in product/tech
  teams)?
- How many teams are involved in the initiative? A single team, several teams working
  on the same product, or several independent teams/products?
- What kind of product/activity (product software, client project, internal platform,
  hardware, regulated sector...)?
- Are there strong dependencies between teams, or can they work largely autonomously?
- Where does the organization stand today: no agile practices, informal ("agile in name
  only"), or an existing transformation already using a framework?

### 2. Resources and culture
- What is the agile maturity level of the teams and management (beginner,
  intermediate, experienced)?
- Is management ready to delegate decisions to teams, or does the culture remain
  very hierarchical/command-and-control?
- Is there budget and dedicated time for training/coaching, or does the framework need
  to be learnable "on the job"?
- Is the pace of work oriented more toward continuous flow (support, operations,
  maintenance) or toward cadenced deliveries/iterations (new products, features)?
- Are there strong predictability/reporting constraints (client commitments,
  steering committee, contractual)?

### 3. Constraints
- Are there regulatory or compliance constraints (health, finance, aerospace...) that
  require traceability, documentation, or validations?
- Is time-to-market critical, or does quality/stability take priority over speed?
- Are there synchronization constraints with other entities (project portfolio,
  other departments, external partners)?
- What is the initiative's horizon: a pilot on a single team, or a rollout at scale
  from the start?

### 4. Ambitions
- What's driving the initiative: improving value delivery, reducing lead times,
  improving quality, improving team engagement, preparing for scaling?
- Is the ambition to evolve a single team, or to structure agility across several
  teams/departments in the medium term?
- Has a cultural preference already been expressed (e.g. "we don't want fixed
  roles", "we want a very simple framework", "we want a framework proven at large
  scale")?

## When to stop

You have enough information once you can answer these 4 questions:
1. How many teams, and are they interdependent?
2. Continuous flow or iterative?
3. Culture: hierarchical/directive or autonomous/collaborative, and agile maturity level?
4. Dominant constraint: predictability/compliance, speed, or quality/engagement?

If the user wants to move fast, you can ask these 4 questions directly instead of the
detailed list above.

## Decision grid

Use this grid as a reasoning guide, not a rigid algorithm: the goal is to arrive at
**one primary recommendation + one alternative**, with justification linking the user's
answers to the choice.

| Dominant signal | Framework(s) to prioritize |
|---|---|
| Single team, product with a clear backlog, iterative pace desired, ambition to establish a regular cadence | **Scrum** |
| Continuous flow of work, high proportion of unplannable requests (support, operations, maintenance), little appetite for formal roles/ceremonies | **Kanban** |
| Single team but culture very averse to fixed roles/process, need for maximum flexibility, product in exploration phase | **Kanban**, or **lightweight Scrum** |
| Several teams (2 to ~5) on the same product, strong dependency between them, need for synchronization without heaviness | **LeSS** (small scale) or **Scrum of Scrums / Nexus** |
| Scaling across many teams, strong predictability constraints (commitments, portfolio, budget), rather hierarchical organization used to formal processes | **SAFe** |
| Scaling across several teams, culture wanting to stay lightweight and avoid process heaviness, priority on team autonomy | **LeSS** or **Spotify Model** (to be adapted, not a fixed framework) |
| Product with long discovery/delivery cycles, senior and autonomous team, wanting to avoid detailed upfront planning (no classic sprint planning) | **Shape Up** |
| Strong regulatory constraints, traceability and documentation mandatory, critical sector (health, aerospace, finance) | **SAFe** or **Scrum with compliance adaptations** (never a "pure" framework that ignores the constraint) |
| Organization at its very first discovery of agility, low maturity, need for a framework simple to teach | **Scrum** (the most documented/tooled to get started), avoiding SAFe at this stage |

Points to explicitly mention in the recommendation:
- **SAFe** is often over-sized for an organization that hasn't yet experimented with
  agility at small scale: proposing it means flagging the risk of heaviness and
  recommending a pilot before rolling it out broadly.
- **Shape Up** assumes an autonomous team and a high level of trust/maturity; it's
  rarely suited to a junior team or a very directive context.
- The "Spotify Model" isn't a prescriptive framework but a source of organizational
  inspiration (tribes/squads): present it as such, never as an off-the-shelf method.
- A hybrid framework (e.g. Scrum at team level + Kanban for support, or Scrum with
  lightened ceremonies) is a legitimate answer if the context is mixed: don't force a
  single choice if reality is hybrid.

## Final recommendation format

Always end with a structured summary:

1. **Context summary** as understood (2-3 sentences, to validate with the user).
2. **Primary recommendation**: the framework, in one clear sentence.
3. **Why**: 3 to 5 points explicitly linking the user's answers to the choice
   (no generic justification).
4. **Alternative to consider**: a second, lighter or more ambitious framework, with the
   condition that would tip the choice toward it.
5. **Risks and points of vigilance**: what could make this choice fail in this
   specific context, and how to anticipate it.
6. **Concrete first steps**: 2-3 actions to get started (e.g. "start with a pilot
   team for 2 sprints before expanding", "train Product Owners before launch").

Keep an advisory tone, not a final verdict: remind the user that the choice can evolve
once tested, and that the important thing is to iterate on the framework itself just as
on the product.
