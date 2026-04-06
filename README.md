# OpenCart Testing Portfolio

A QA portfolio project covering API, performance, and UI testing.

## Tools Used
- Postman (API Testing)
- JMeter (Performance Testing)
- Selenium (UI Testing)

## Project Structure
- `postman/` — API test collection and environment for Restful Booker
- `jmeter/` — Performance test plans and reports for OpenCart
- `selenium/` — UI automation scripts for OpenCart
- `bug-reports/` — Documented bugs found during testing

## API Testing (Restful Booker)
- CRUD operations (Create, Read, Update, Delete bookings)
- Chained requests using environment variables
- Auto token refresh via Pre-request script
- Assertions on status codes, response body, and response time
- Negative test cases (invalid inputs, missing fields, wrong token)
- 1 bug found and documented

### Results
![API Test Results](screenshots/api-test-results.png)

## Performance Testing (OpenCart)

### Test Scenarios
| Scenario | Users | Avg Response | Error Rate |
|---|---|---|---|
| Smoke Test | 2 | 137ms | 0.00% |
| Load Test - Low | 10 | 147ms | 0.00% |
| Load Test - Medium | 50 | 122ms | 0.00% |
| Load Test - High | 100 | 129ms | 0.00% |
| Stress Test | 200 | 120ms | 0.00% |

### Key Findings
- OpenCart handled up to 200 concurrent users with 0% error rate
- Average response time stayed under 150ms across all scenarios
- APDEX score of 1.000 — perfect user satisfaction rating
- No performance degradation detected under stress conditions

  
## Status
🟡 In Progress
