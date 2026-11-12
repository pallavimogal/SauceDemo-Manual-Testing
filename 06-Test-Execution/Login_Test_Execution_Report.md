# SauceDemo — Login Test Execution Report

## 1. Execution Information
- Project: SauceDemo Manual Testing
- Module: Login & Authentication
- Tester: Pallavi Mogal
- Execution Date: 11/11/2026


## 2. Execution Summary

| Metric | Count |
|---|---|
| Total Planned | 5 |
| Passed | 5 |
| Failed | 0 |
| Blocked | 0 |
| Not Run | 0 |

## 3. Detailed Execution Results

| Test Case ID | Status | Actual Result | Evidence |
|---|---|---|---|
| TC_LOGIN_001 | Pass | Login successful; inventory page displayed   | TC_LOGIN_001.png |
| TC_LOGIN_002 | Pass | Login was rejected when an invalid password was entered. The application displayed the error message "Epic sadface: Username and password do not match any user in this service." The user remained on the login page. | TC_LOGIN_002.png |
| TC_LOGIN_003 | Pass | Login was rejected when an invalid username was entered. The application displayed the error message "Epic sadface: Username and password do not match any user in this service." The user remained on the login page. | TC_LOGIN_003.png |
| TC_LOGIN_004 | Pass | The application prevented the login attempt when the username field was left blank and displayed the validation message "Epic sadface: Username is required." The user remained on the login page, and access to the inventory page was not granted. | TC_LOGIN_004.png |
| TC_LOGIN_005 | Pass | The application prevented the login attempt when the password field was left blank and displayed the validation message "Epic sadface: Password is required." The user remained on the login page, and access to the inventory page was not granted. | TC_LOGIN_005.png |


## 4. Execution Conclusion 

All 5 planned login test cases were executed successfully, achieving a 100% pass rate. The application behaved as expected for valid credentials, invalid credentials, and mandatory-field validation scenarios. No failures were observed within the executed login test cases.
