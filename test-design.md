# Functional Test Cases

| TC ID | Scenario               | Test Data                   | Expected Result         |
| ----- | ---------------------- | --------------------------- | ----------------------- |
| TC001 | Successful transfer    | Amount=500 GBP              | Transfer successful     |
| TC002 | Unsupported currency   | Currency=NGN                | Error returned          |
| TC003 | Insufficient balance   | Amount greater than balance | Error returned          |
| TC004 | Invalid wallet ID      | Invalid sender wallet       | Error returned          |
| TC005 | Transfer above £5,000  | Amount=6000 GBP             | Approval required       |
| TC006 | Above maximum limit    | Amount=10000.01 GBP         | Error returned          |
| TC007 | Duplicate transaction  | Same request twice          | Second request rejected |
| TC008 | Missing required field | No receiverWalletId         | Validation error        |
| TC009 | Unauthorized request   | No auth token               | 401 Unauthorized        |


# Boundary Value Analysis

| Amount     | Expected Result   |
| ---------- | ----------------- |
| £0         | Fail              |
| £1         | Pass              |
| £4,999.99  | Pass              |
| £5,000     | Pass              |
| £5,000.01  | Approval Required |
| £9,999.99  | Pass              |
| £10,000    | Pass              |
| £10,000.01 | Fail              |

