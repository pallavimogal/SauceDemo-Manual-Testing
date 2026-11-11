# SauceDemo — Detailed Manual Test Cases

**Project:** SauceDemo Manual Testing  
**Document ID:** STC-001  
**Version:** 1.0  
**Prepared By:** Pallavi Mogal  
**Status:** Draft — Test Design

## Test Case Summary

| Test Case ID | Scenario ID | Test Case Title | Priority | Status |
|---|---|---|---|---|
| TC_LOGIN_001 | TS_LOGIN_01 | Verify successful login with valid credentials | High | Not Run |
| TC_LOGIN_002 | TS_LOGIN_02 | Verify login with invalid password | High | Not Run |
| TC_LOGIN_003 | TS_LOGIN_03 | Verify login with invalid username | High | Not Run |
| TC_LOGIN_004 | TS_LOGIN_04 | Verify login with blank username | High | Not Run |
| TC_LOGIN_005 | TS_LOGIN_05 | Verify login with blank password | High | Not Run |

---

## TC_LOGIN_001 — Verify Successful Login

**Scenario ID:** TS_LOGIN_01  
**Module:** Login & Authentication  
**Priority:** High  
**Test Type:** Positive / Functional

**Preconditions:**
- SauceDemo login page is accessible.
- User is logged out.

**Test Data:**
- Username: standard_user
- Password: secret_sauce

**Test Steps:**
1. Navigate to https://www.saucedemo.com/.
2. Enter standard_user in Username.
3. Enter secret_sauce in Password.
4. Click Login.

**Expected Result:** The user successfully logs in, is redirected to the inventory page, and can view the product list.

**Actual Result:** Not recorded  
**Status:** Not Run  
**Evidence:** Not captured

---

## TC_LOGIN_002 — Verify Invalid Password

**Scenario ID:** TS_LOGIN_02  
**Module:** Login & Authentication  
**Priority:** High  
**Test Type:** Negative / Functional

**Preconditions:**
- SauceDemo login page is accessible.

**Test Data:**
- Username: standard_user
- Password: wrong123

**Test Steps:**
1. Navigate to the SauceDemo login page.
2. Enter standard_user in Username.
3. Enter wrong123 in Password.
4. Click Login.

**Expected Result:** Login is rejected, an appropriate authentication error appears, and the user is not redirected to inventory.

**Actual Result:** Not recorded  
**Status:** Not Run  
**Evidence:** Not captured

---

## TC_LOGIN_003 — Verify Invalid Username

**Scenario ID:** TS_LOGIN_03  
**Module:** Login & Authentication  
**Priority:** High  
**Test Type:** Negative / Functional

**Preconditions:**
- SauceDemo login page is accessible.

**Test Data:**
- Username: invalid_user
- Password: secret_sauce

**Test Steps:**
1. Navigate to the SauceDemo login page.
2. Enter invalid_user in Username.
3. Enter secret_sauce in Password.
4. Click Login.

**Expected Result:** Login is rejected, an appropriate authentication error appears, and the user remains unauthenticated.

**Actual Result:** Not recorded  
**Status:** Not Run  
**Evidence:** Not captured

---

## TC_LOGIN_004 — Verify Blank Username

**Scenario ID:** TS_LOGIN_04  
**Module:** Login & Authentication  
**Priority:** High  
**Test Type:** Negative / Required Field Validation

**Preconditions:**
- SauceDemo login page is accessible.

**Test Data:**
- Username: Blank
- Password: secret_sauce

**Test Steps:**
1. Navigate to the SauceDemo login page.
2. Leave Username blank.
3. Enter secret_sauce in Password.
4. Click Login.

**Expected Result:** Login is prevented and a message indicates that the username is required.

**Actual Result:** Not recorded  
**Status:** Not Run  
**Evidence:** Not captured

---

## TC_LOGIN_005 — Verify Blank Password

**Scenario ID:** TS_LOGIN_05  
**Module:** Login & Authentication  
**Priority:** High  
**Test Type:** Negative / Required Field Validation

**Preconditions:**
- SauceDemo login page is accessible.

**Test Data:**
- Username: standard_user
- Password: Blank

**Test Steps:**
1. Navigate to the SauceDemo login page.
2. Enter standard_user in Username.
3. Leave Password blank.
4. Click Login.

**Expected Result:** Login is prevented and a message indicates that the password is required.

**Actual Result:** Not recorded  
**Status:** Not Run  
**Evidence:** Not captured

---

## Execution Notes

- All cases are currently in Not Run status.
- Actual results and evidence will be recorded during execution.
- Expected behaviors are initial testing expectations and will be reviewed against available requirements.
- No defect has been reported or confirmed at this stage.
