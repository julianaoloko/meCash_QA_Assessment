Security & Compliance Testing Approach

## Authentication

Authentication testing verifies that only authorised users can access the Fund Transfer API. The testing process will involve sending requests with valid credentials, as well as scenarios involving missing, expired, and invalid tokens. The expected outcome is that unauthorised requests are rejected, accompanied by an appropriate error response.

## Authorization

Authorisation testing verifies that users can only perform actions they are permitted to execute. Tests will confirm that a user cannot initiate transfers from wallets that do not belong to them and cannot access other users' transaction data.

## Rate Limiting

Rate-limiting tests will be performed by sending a high volume of requests within a short period. The objective is to verify that the API restricts excessive requests and returns the appropriate throttling response when limits are exceeded.

## Input Validation

Input validation testing ensures the API properly handles invalid data. Test scenarios include negative transfer amounts, empty wallet identifiers, unsupported currencies, special characters, and excessively large payloads. The API should reject invalid input and return meaningful validation messages.

## PCI DSS Compliance.

To comply with PCI DSS requirements, testing will confirm that sensitive payment information is encrypted during both transmission and storage. Additionally, logs and error messages will be examined to ensure that sensitive financial data is not exposed.

## GDPR Compliance
GDPR testing emphasises the protection of personal data. The verification process will include ensuring that personal information is handled securely, that only necessary data is stored, and that data retention practices comply with regulatory requirements.

## Audit Logging

Audit logging tests will ensure that every successful transfer creates an audit record with relevant transaction details, timestamps, and user information. These logs must support traceability and compliance requirements.
