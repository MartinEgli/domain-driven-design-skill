# Example Order Domain DDD

## Input

Model an order management domain with payment and fulfillment.

## Output Shape

- Subdomains:
  - Ordering: core
  - Payment: supporting or generic, depending on business model
  - Fulfillment: supporting
- Bounded contexts:
  - Ordering
  - Payment
  - Fulfillment
  - Returns
- Aggregates:
  - Order protects order line and state transition invariants
  - PaymentIntent protects authorization/capture invariants
  - Shipment protects fulfillment status
- Domain events:
  - OrderPlaced
  - PaymentAuthorized
  - ShipmentCreated
  - ReturnRequested
- Context map:
  - Ordering upstream to Fulfillment via Published Language
  - Payment upstream to Ordering for authorization state
- Open questions:
  - Who owns customer credit decision?
  - Can partial shipment happen?
  - Which return states are legal?
