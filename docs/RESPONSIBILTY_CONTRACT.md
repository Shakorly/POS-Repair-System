# Backend $ FrantEnd Responsibilty Contract 

## Core Rule
Frontend requests => Bankend Decides => Database enforces

-------------------------------------

## Fronted Responsibilities

- Collect user input
- DIsplay user input 
- Trigger HTTP requests
- Never enforce business rules
- Never assume success
- Never modify state locally 

-------------------------------------

## Backend Responsibilties

- Validate all input
- Enforce all business rules
- Control repair state transitions 
- Enforce authorization 
- Log every critical action 
- Persist and protect data

--------------------------------------

### Forbidden Practice 
- No business login in frontend 
- No database access from controller
- No deletes without audit
- No trusting client input 
- No skipping valudation

---------------------------------------

## Deployment Rule 

- Ony backed is the source of truth
- Front reflects backend state only
- Separate front and bacjk end folder