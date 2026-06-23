# Evidence And Traceability

Use this reference whenever DDD model elements, diagrams, context maps, or
recommendations depend on supplied inputs.

## Input Register

Track meaningful inputs by source type:

- User fact: stated directly by the user.
- Artifact: workshop note, event storming board, process description, glossary,
  schema, code, API contract, support ticket, domain document, or diagram.
- Tool result: query output, code search result, test result, generated report,
  or extracted event/command list.
- External source: cited domain policy, regulation, standard, or public source.
- Assumption: useful but unverified domain hypothesis.

## Traceability Rules

- Preserve domain terms, event names, commands, actors, policies, and invariants
  exactly unless explicitly refining language.
- Tie each bounded context, aggregate, event, invariant, and relationship to a
  source or mark it as a hypothesis.
- Do not promote database tables, screens, or DTOs to domain truth without
  domain evidence.
- Mark missing domain expert input as a gap.
- Keep conflicting language visible instead of silently normalizing it.

## Evidence Receipt

For substantial outputs, include a compact receipt:

| Model Element Or Decision | Source/Input | Type | Confidence | Gap Or Follow-up |
| --- | --- | --- | --- | --- |

Use `not supplied` when the input is missing. Use `hypothesis` for unverified
model elements.

## Verification Pattern

Follow the small-loop pattern:

1. Locate relevant domain language, processes, rules, events, and invariants.
2. Make the smallest scoped model proposal.
3. Verify the output against evidence, hypotheses, domain questions, and skill
   boundaries.

Avoid DDD ceremony that is not supported by domain complexity or supplied
evidence.
