# DDD Review Reference

Use this reference for `/ddd review`.

## Review Focus

- Ubiquitous language: terms are business-facing, consistent, and not merely
  technical names.
- Bounded contexts: each context has a clear model, responsibility, owner, and
  integration relationship.
- Subdomains: core, supporting, and generic subdomains are separated and tied to
  strategic value.
- Aggregates: aggregate boundaries protect real invariants and avoid excessive
  transaction scope.
- Domain events: events describe business facts that happened, with clear
  producer, consumer, and ownership.
- Service split: services follow domain boundaries rather than technical layers
  or database tables by default.
- Legacy decomposition: strangler, anti-corruption, migration, and data
  ownership concerns are explicit when relevant.

## Review Signals

Watch for:

- objects named after screens, tables, frameworks, or transport contracts
- aggregates with no invariant
- events named as commands or technical notifications
- shared database ownership across bounded contexts
- context names that duplicate team names without a model boundary
- microservice splits made before language and invariants are understood

## Output Expectations

- Separate evidence, inference, assumption, and gap.
- State whether each issue is strategic DDD, tactical DDD, or software
  architecture.
- Hand deployment, API style, Clean Architecture, or quality attribute concerns
  to `software-architecture`.
- Hand capability, portfolio, and roadmap concerns to `enterprise-architecture`.
- End with the highest-value domain expert questions.
