# POS Repair System — Business Rules

## Repair Workflow Rules

1. A POS terminal MUST be assigned before repair can start.
2. A technician cannot work on more than 20 terminals at once.
3. A repair MUST be started before it can be completed.
4. A repair MUST be completed before it can be sent to QA.
5. Repairs can NEVER be deleted — only archived.
6. Every state change MUST be logged for audit purposes.
7. Unrepairable pos are sent back to inventory

## Security Rules

1. Frontend input is NEVER trusted.
2. Backend is the single source of truth.
3. Authorization is role-based (Technician, QA, Inventory).
