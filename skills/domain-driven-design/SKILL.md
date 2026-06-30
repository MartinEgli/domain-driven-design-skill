---
name: domain-driven-design
description: >
  Domain-Driven Design skill for strategic DDD, tactical DDD, bounded contexts,
  context maps, subdomain classification, ubiquitous language, aggregates,
  entities, value objects, domain services, domain events, repositories, event
  storming, model discovery, legacy decomposition, and aligning software design
  with complex business domains, including Mermaid, PlantUML, context map,
  aggregate, domain event, and event storming diagrams.
---

# Domain-Driven Design

## Purpose

Use Domain-Driven Design to understand a complex domain, create shared language,
shape bounded contexts, define model boundaries, and produce useful software
design decisions.

## When to Use

Use when the user asks for:

- bounded contexts
- context mapping
- subdomain classification
- ubiquitous language
- aggregate design
- domain events
- event storming
- service decomposition by domain
- legacy system decomposition
- DDD review of architecture or code
- domain model refinement
- DDD diagrams such as context maps, subdomain maps, aggregate boundaries,
  domain event flows, event storming summaries, or ubiquitous language maps

## Do Not Use When

Do not use DDD ceremony for simple CRUD, simple workflow, or low-domain-complexity
tasks. Use `software-architecture` for broader software design without deep
domain modeling.

Do not use for enterprise capability maps, portfolio rationalization, operating
model, or roadmap decisions. Use `enterprise-architecture` for those.

Do not use for final evidence acceptance, architecture gate approval, or
productive-use governance of AI-generated model claims. Use
`mournival-architecture` for those.

## Mandatory Rules

- Start from domain language, business process, and invariants.
- Separate strategic DDD from tactical DDD.
- Do not design aggregates before bounded contexts and invariants are clear.
- Do not split services by technical layer when domain boundaries are unclear.
- Preserve user-provided domain terms exactly unless asking to refine them.
- Mark assumptions, open questions, and missing domain expert input.
- Keep domain model elements, diagrams, and recommendations traceable to domain
  language, supplied artifacts, sources, or clearly marked assumptions.
- Prefer useful models over perfect models.
- When creating diagrams, stay within DDD model scope and read
  `references/diagrams.md`.
- Escalate software architecture concerns to `software-architecture` when the
  question becomes about deployment, API style, quality attributes, or Clean
  Architecture beyond DDD.
- Escalate capability, portfolio, roadmap, or operating model questions to
  `enterprise-architecture`.
- If domain expert input, invariant, or business outcome is missing, mark the
  model as a hypothesis and show the question that must be answered.

## Inputs Expected

- domain description
- business process or value stream
- actors and roles
- commands and decisions
- events and outcomes
- policies and rules
- data concepts
- invariants
- pain points
- current systems or teams

## Modes

### /ddd discover

Extract domain language, actors, commands, events, policies, invariants, and
open questions. Read `references/discovery.md`.

### /ddd context-map

Identify bounded contexts and relationships such as customer/supplier,
conformist, shared kernel, anti-corruption layer, and separate ways. Read
`references/context-mapping.md`.

### /ddd subdomains

Classify core, supporting, and generic subdomains. Identify strategic focus and
build/buy/partner implications. Read `references/strategic-ddd.md`.

### /ddd aggregate

Design aggregates around invariants, consistency boundaries, commands, and
domain events. Read `references/tactical-ddd.md`.

### /ddd events

Identify domain events, event names, producers, consumers, payload ownership,
and downstream policy reactions. Read `references/domain-events.md`.

### /ddd event-storm

Prepare or summarize an event storming model. Read `references/event-storming.md`.

### /ddd review

Review an existing model, service split, or code structure against DDD
principles. Read `references/ddd-review.md`.

### /ddd diagram

Create or review DDD diagrams using Mermaid, PlantUML, or lightweight
modeling notation: context maps, subdomain maps, aggregate boundaries, event
flows, or event storming summaries. Read `references/diagrams.md`.


### /domain-driven-design feedback

Capture lessons from the current run without changing the skill automatically.
Use eferences/feedback-route.md to classify user feedback, observed gaps,
assumptions, candidate improvements, rejected ideas, and routed follow-ups.

### /domain-driven-design improve

Review accumulated feedback and propose concrete skill changes. Use
ssets/improvement-proposal-template.md. Do not modify behavior until the
proposal names evidence, affected files, risks, validation commands, versioning
impact, and rollback considerations.
## Evidence Handling
Use `references/evidence-traceability.md`.
Use eferences/feedback-route.md when capturing or applying lessons from a run.

- Evidence: supplied domain language, process, event, rule, code, schema,
  workshop note, or explicit user fact.
- Inference: proposed model element derived from evidence.
- Assumption: useful but unverified domain hypothesis.
- Gap: missing domain expert input or business rule.

Include an Evidence Receipt for substantial findings, decisions, diagrams, or
recommendations.

## Output Contracts

Use `assets/templates/ddd-output-template.md` unless user asks for another
format.

## Quality Gates

- Ubiquitous language terms are explicit.
- Bounded contexts have clear responsibility.
- Context relationships are named.
- Aggregates protect real invariants.
- Domain events are business facts, not technical notifications.
- Open domain questions are visible.
- Model elements include source trace or are marked as hypotheses.
- Tactical design does not outrun strategic boundaries.
- Diagrams use domain language and mark hypotheses when domain expert evidence
  is missing.

## Boundaries

- Do not claim domain truth without domain expert evidence.
- Do not invent business rules.
- Do not force event sourcing or microservices.
- Do not treat database tables as the domain model by default.


## Continuous Improvement

This skill is self-improving only through an explicit, auditable feedback loop:
feedback -> evidence -> improvement proposal -> feature branch -> validation ->
commit -> push -> version or changelog update when needed. Do not silently alter
skill behavior based on a single run. Preserve rejected and deferred ideas so
future maintainers can see why they were not applied.
## Output Style
- Use concrete domain terms.
- Prefer concise tables and bullet lists.
- Prefer Mermaid for quick domain modeling diagrams and PlantUML when the user
  wants persistent model diagrams.
- Keep model hypotheses visibly marked.
- End with open questions and next modeling actions.
