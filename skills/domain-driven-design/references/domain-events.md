# Domain Events

Domain events are business facts that already happened.

## Naming

Use past tense business language:

- OrderPlaced
- PaymentAuthorized
- ShipmentCreated
- ReturnRequested

Avoid technical names:

- OrderUpdated
- RecordSaved
- MessageSent

## Checks

- What business fact happened?
- Who cares downstream?
- Which aggregate produced it?
- What minimal payload is needed?
- Is payload ownership clear?
- Is event versioning needed?
- Does the event trigger a policy?

Domain events are not a replacement for all integration design. Escalate broader
integration concerns to `software-architecture`.
