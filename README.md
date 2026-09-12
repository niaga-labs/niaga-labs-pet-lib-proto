# lib-proto

Shared event schemas and DTOs for Kilat Pet Runner.

## Organization

[github.com/niaga-labs](https://github.com/niaga-labs)

## What It Provides

### Events (CloudEvent schemas for Kafka topics)

- **booking.events** — Booking lifecycle (6 events)
  - Requested, Accepted, PickedUp, DeliveryConfirmed, Completed, Cancelled

- **payment.events** — Payment processing (5 events)
  - EscrowCreated, Held, Released, Refunded, PaymentFailed

- **runner.events** — Runner status (4 events)
  - Online, Offline, LocationUpdate, Assigned

- **tracking.events** — Order tracking (3 events)
  - Started, Updated, Completed

### DTOs (Shared cross-service data structures)

User, Runner, CrateSpec, Address, PetSpec, Vaccination, Coordinate

## Installation

```bash
go get github.com/niaga-labs/niaga-labs-pet-lib-proto
```

## Requirements

- Go 1.24+
