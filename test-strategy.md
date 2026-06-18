# Test Strategy

## Objective

To verify that the Fund Transfer API processes transfers correctly and enforces all business rules.

## Scope

Endpoint:
POST /api/v1/transfers

## Test Types

### Functional Testing

Validate transfer creation, approval requirements, supported currencies, and transaction limits.

### Negative Testing

Verify that invalid requests are rejected appropriately.

### Boundary Testing

Validate behaviour at minimum, maximum, and approval threshold values.

### Security Testing

Validate authentication, authorisation, input validation, and rate limiting requirements.

## Test Scenarios

1. Successful Transfer
2. Unsupported Currency
3. Invalid amount
4. Invalid Wallet ID
5. Missing Required Field


## Entry Criteria

* API specification available
* Mock API configured

## Exit Criteria

* All planned test cases executed
* Critical defects documented
* Test execution report completed
