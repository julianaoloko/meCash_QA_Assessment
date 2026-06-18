# meCash_QA_Assessment
This repo was created to give a full analysis of mock datasets for a QA Assessment.

# Fund Transfer API Assessment

## Overview

This project contains the test design, API test scenarios, security considerations, and CI/CD proposal for the Fund Transfer API assessment.

## Objective

To validate that the Fund Transfer API correctly processes transfers while enforcing all defined business rules and security requirements.

## Assumptions

* No Base URL was provided in the API specification.
* No authentication endpoint or token generation process was provided.
* Mockaroo was used to generate mock API data and simulate API responses.
* Error scenarios such as 400 Bad Request, 401 Unauthorised, and 409 Conflict were documented as expected outcomes.

## Tools Used

* Postman
* Mockaroo
* GitHub
* GitHub Actions

## Test Coverage

### Functional Testing

* Successful transfer
* Unsupported currency
* Invalid wallet ID
* Missing required fields


### Boundary Value Analysis

* £0
* £1
* £4,999.99
* £5,000
* £5,000.01
* £9,999.99
* £10,000
* £10,000.01

### Security Testing

* Authentication
* Authorization
* Input validation
* Rate limiting
* Audit logging



