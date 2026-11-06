# Test Plan — Online Banking Application — Manual Test Documentation

## 1. Introduction
This plan describes how the **Online Banking Application — Manual Test Documentation** will be tested manually. Application under test: a demo internet-banking application (login, balance, fund transfer, statement, PIN change).

## 2. Scope
**In scope**
- Login & session security
- Account balance
- Fund transfer & OTP
- Statement
- Profile / PIN change
- Access control

**Out of scope:** performance/load testing, security penetration testing, third-party payment gateway internals.

## 3. Test Approach
- Test levels: Smoke -> Functional -> Regression -> Exploratory -> UAT
- Design techniques: Equivalence Partitioning, Boundary Value Analysis, Decision Table, Error Guessing
- Test types: Functional, Usability, Compatibility (Chrome / Firefox / Edge), Negative testing

## 4. Entry Criteria
- Requirements reviewed and baselined; test environment and test data ready; build deployed and smoke test passed.

## 5. Exit Criteria
- 100% of high-priority test cases executed; no open Critical/High defects; all deviations documented.

## 6. Defect Management
Defects are logged with the template in `bug-report-template.md` and follow the life cycle:
New -> Assigned -> Open -> Fixed -> Retest -> Verified -> Closed (or Reopened / Rejected / Deferred).
Severity: Blocker, Critical, Major, Minor, Trivial. Priority: P1 (fix now), P2, P3.

## 7. Test Deliverables
Test plan, test scenarios, test cases (`test-cases.csv`), RTM, bug reports, test summary report.

## 8. Risks & Mitigation
| Risk | Mitigation |
|---|---|
| Requirements change late | Re-run impact analysis, update RTM |
| Test data unavailable | Prepare data sets before execution |
| Tight schedule | Execute by priority (P1 first) |
