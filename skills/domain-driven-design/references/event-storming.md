# Event Storming

Use event storming to discover domain flow with domain experts.

## Elements

- Domain Event: important business fact.
- Command: intent to make something happen.
- Actor: role issuing command.
- Policy: rule reacting to event.
- Aggregate: consistency boundary handling command.
- External System: outside participant.
- Hotspot: uncertainty, conflict, or risk.

## Flow

1. List domain events in timeline order.
2. Add commands that cause events.
3. Add actors issuing commands.
4. Add policies reacting to events.
5. Identify aggregates and bounded contexts.
6. Mark hotspots and questions.

Do not turn workshop artifacts into final design without review.
