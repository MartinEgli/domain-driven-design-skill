# Tactical DDD

Use tactical DDD after bounded context and language are sufficiently clear.

## Building Blocks

- Entity: object with identity and lifecycle.
- Value Object: immutable descriptive value without identity.
- Aggregate: consistency boundary protecting invariants.
- Aggregate Root: entry point for aggregate changes.
- Domain Service: domain operation that does not belong naturally to one entity
  or value object.
- Repository: collection-like access to aggregate roots.

## Aggregate Checks

- Which invariant must always hold?
- Which command changes the aggregate?
- Which data must be strongly consistent?
- Which rules can become eventually consistent?
- Which domain event follows successful change?
- Is the aggregate too large because it mirrors a database table?

Do not design aggregates as object graphs. Design them as consistency
boundaries.
