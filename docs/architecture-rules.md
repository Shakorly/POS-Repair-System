# Architecture Rules

## General Rules

1. Controllers contain ZERO business logic.
2. Services enforce all business rules.
3. Controllers NEVER talk directly to the database.
4. All state changes happen inside services.
5. DTOs(Data Transfer Object) validate data at the system boundary.
6. No hard deletes — archive instead.

## Frontend Rules

1. UI never updates optimistically.
2. UI always reflects backend-confirmed state.
3. Fetch layer is separated from UI logic.

## Backend Rules

1. Modules are designed before entities.
2. Guards are used for authorization, not if-statements.
3. synchronize: true is NEVER used in production.
