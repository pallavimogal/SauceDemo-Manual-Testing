# Manual Test Plan — SauceDemo

## 1. Document Information
- Project Name: SauceDemo Manual Testing
- Application Under Test: SauceDemo (Swag Labs)
- Test Plan ID: STP-001
- Version: 1.0
- Prepared By: Pallavi Mogal
- Project Type: Independent QA Portfolio
- Status: Draft

## 2. Objective
The objective is to validate the key functional workflows of the SauceDemo e-commerce application, identify reproducible defects, and document test execution results.

## 3. Scope of Testing
### In Scope
- Login with valid and invalid credentials
- Product inventory display
- Product sorting
- Product details
- Add and remove products from the shopping cart
- Cart item and quantity verification
- Checkout information validation
- Checkout overview and order confirmation
- Logout functionality
- Positive and negative testing

### Out of Scope
- Real payment gateway processing
- Backend database validation
- Performance and load testing
- Security penetration testing
- Mobile application testing
- Production integration testing

## 4. Test Approach
Manual functional testing will be performed using:
- Positive and negative testing
- Equivalence partitioning
- Boundary value analysis where applicable
- Exploratory testing
- Regression testing of relevant workflows

Test cases will contain prerequisites, test steps, test data, expected results, actual results, and execution status.

## 5. Test Environment
- Application URL: https://www.saucedemo.com/
- Environment: Public demonstration website
- Platform: Web browser
- Browser and Version: To be recorded during execution
- Operating System: To be recorded during execution
- Test Credentials: Publicly supplied demo credentials

## 6. Entry Criteria
- SauceDemo application is accessible
- Test scope and expected behavior are documented
- Test cases are reviewed for completeness
- Required demo credentials are available
- Test environment is ready

## 7. Exit Criteria
- All planned test cases have been executed or marked Blocked/Not Run with reasons
- Execution results and evidence are documented
- Reproducible defects are recorded
- Outstanding issues and limitations are summarized
- Final test execution summary is prepared

## 8. Defect Management
Defects will be documented with:
- Defect ID
- Title and description
- Module
- Environment
- Steps to reproduce
- Expected result
- Actual result
- Severity and priority
- Screenshots or evidence
- Status

Defect status will be tracked in project documentation.

## 9. Test Deliverables
- Manual Test Plan
- Test Scenarios
- Detailed Test Cases
- Test Execution Report
- Defect Reports, if applicable
- Screenshots and Test Evidence
- Requirements Traceability Matrix
- Test Summary Report

## 10. Risks and Mitigation
| Risk | Mitigation |
| --- | --- |
| Public demo website is unavailable | Record the blocker and resume when available |
| Expected behavior is undocumented | Record assumptions and distinguish them from confirmed requirements |
| Shared demo data changes unexpectedly | Reset the application state before relevant tests |
| Test evidence is incomplete | Capture results and screenshots during execution |

## 11. Roles and Responsibilities
Independent QA Tester — Pallavi Mogal

Responsibilities:
- Analyze application functionality
- Prepare testing documentation
- Design and execute manual test cases
- Record defects and supporting evidence
- Prepare test execution and summary reports

## 12. Test Schedule
- Phase 1: Application exploration and planning
- Phase 2: Test scenario preparation
- Phase 3: Test case design
- Phase 4: Manual test execution
- Phase 5: Defect documentation
- Phase 6: Test summary and GitHub publication

## 13. Assumptions and Limitations
This is an independent portfolio project. Official business requirements, source code, and backend services are not available. Expected results will be based on observed application behavior and explicitly documented assumptions. No testing has been executed at the time this initial plan is created.
