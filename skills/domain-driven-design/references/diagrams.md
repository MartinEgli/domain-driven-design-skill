# Domain-Driven Design Diagrams

Use this reference for `/ddd diagram` or when the user asks for a DDD diagram.

## Scope

Create diagrams for domain modeling:

- bounded context maps
- subdomain maps: core, supporting, generic
- upstream/downstream and context relationship diagrams
- aggregate boundaries and invariant ownership
- command, policy, and domain event flows
- event storming summaries
- ubiquitous language maps
- legacy decomposition and anti-corruption layer diagrams

Hand deployment, API style, Clean Architecture, component, and detailed runtime
sequence diagrams to `software-architecture`. Hand capability, portfolio, or
roadmap diagrams to `enterprise-architecture`.

## Notation Choice

- Mermaid `flowchart` for context maps, subdomain maps, event flows, and
  aggregate sketches.
- Mermaid `sequenceDiagram` only when showing domain interaction order, not
  technical transport detail.
- PlantUML component/object-style diagrams when the user wants persistent DDD
  diagrams or stronger notation.
- Keep event storming diagrams simple: command -> aggregate/policy -> event ->
  downstream policy/read model.

## Diagram Rules

- Use domain language, not technical table or screen names by default.
- Mark hypotheses when domain expert confirmation is missing.
- Do not design aggregates before invariants are clear.
- Do not imply microservices just because bounded contexts exist.
- Name context relationships: customer/supplier, conformist, shared kernel,
  anti-corruption layer, open host service, published language, or separate
  ways.

## Output Pattern

1. State modeling purpose and diagram type.
2. State notation used and why.
3. Provide diagram code.
4. List domain terms, invariants, and context relationships.
5. End with domain expert questions and model risks.
