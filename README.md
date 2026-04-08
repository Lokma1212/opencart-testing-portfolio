# OpenCart Testing Portfolio

A comprehensive QA portfolio project covering API, Performance, and UI testing.

**Tools:** Postman | JMeter | Selenium | Python  
**Portfolio Link:** https://github.com/Lokma1212/opencart-testing-portfolio

---

## API Testing (Restful Booker)
**Tool:** Postman  
**Test Cases:** 9 (5 positive + 4 negative)  
**Assertions:** 15  
**Result:** 15/15 passing ✅

### What was tested:
- CRUD operations (Create, Read, Update, Delete bookings)
- Chained requests with automatic booking ID capture
- Auto token refresh via Pre-request script
- Assertions on status codes, response body, and response time
- Negative cases: invalid ID, missing fields, wrong token, no token

### Bug Found:
- **Bug 001:** POST /booking returns 500 instead of 400 when required fields are missing

![API Test Results](screenshots/api-test-results.png)

---

## Performance Testing (OpenCart)
**Tool:** JMeter  
**Mode:** GUI + Non-GUI (CLI)

### Test Scenarios:
| Scenario | Users | Avg Response | Error Rate |
|---|---|---|---|
| Smoke Test | 2 | 137ms | 0.00% |
| Load Test - Low | 10 | 147ms | 0.00% |
| Load Test - Medium | 50 | 122ms | 0.00% |
| Load Test - High | 100 | 129ms | 0.00% |
| Stress Test | 200 | 120ms | 0.00% |

### Key Findings:
- OpenCart handled up to 200 concurrent users with 0% error rate
- Average response time stayed under 150ms across all scenarios
- APDEX score of 1.000 — perfect user satisfaction rating
- No performance degradation detected under stress conditions

---

## UI Testing (OpenCart)
**Tool:** Selenium + Python (Jupyter Notebook)  
**Test Cases:** 5  
**Result:** 5/5 passing ✅

### What was tested:
- Homepage loads correctly
- Product search functionality
- Add product to cart
- New user registration
- User login

---

## Bug Reports
| ID | Endpoint | Expected | Actual | Severity |
|---|---|---|---|---|
| Bug-001 | POST /booking | 400 Bad Request | 500 Internal Server Error | Medium |

---

## Status
🟢 Complete
