# SauceDemo — Manual Test Scenarios

**Project:** SauceDemo Manual Testing
**Document ID:** STS-001
**Version:** 1.0
**Author:** Pallavi Mogal
**Status:** Draft — Test Design

## Objective
Identify functional test scenarios for the SauceDemo application, covering positive, negative, and workflow validation.

## Test Scenario List

| Scenario ID | Module | Test Scenario | Test Type |
|---|---|---|---|
| TS_LOGIN_01 | Login | Verify login with valid credentials | Positive |
| TS_LOGIN_02 | Login | Verify login with an invalid password | Negative |
| TS_LOGIN_03 | Login | Verify login with an invalid username | Negative |
| TS_LOGIN_04 | Login | Verify login with a blank username | Negative |
| TS_LOGIN_05 | Login | Verify login with a blank password | Negative |
| TS_INV_01 | Inventory | Verify available products are displayed | Functional |
| TS_INV_02 | Inventory | Verify product names and prices are displayed | Functional |
| TS_INV_03 | Inventory | Verify navigation to product details | Functional |
| TS_INV_04 | Inventory | Verify product images are displayed | Functional |
| TS_INV_05 | Inventory | Verify navigation back to inventory | Functional |
| TS_SORT_01 | Sorting | Verify sorting by name A to Z | Functional |
| TS_SORT_02 | Sorting | Verify sorting by name Z to A | Functional |
| TS_SORT_03 | Sorting | Verify sorting by price low to high | Functional |
| TS_SORT_04 | Sorting | Verify sorting by price high to low | Functional |
| TS_SORT_05 | Sorting | Verify changing the selected sorting option | Functional |
| TS_CART_01 | Cart | Verify adding one product to the cart | Positive |
| TS_CART_02 | Cart | Verify adding multiple products | Positive |
| TS_CART_03 | Cart | Verify removing a product | Functional |
| TS_CART_04 | Cart | Verify cart badge updates | Functional |
| TS_CART_05 | Cart | Verify cart item details and quantities | Functional |
| TS_CHK_01 | Checkout | Verify checkout with valid information | Positive |
| TS_CHK_02 | Checkout | Verify blank first name validation | Negative |
| TS_CHK_03 | Checkout | Verify blank last name validation | Negative |
| TS_CHK_04 | Checkout | Verify blank postal code validation | Negative |
| TS_CHK_05 | Checkout | Verify order summary details and pricing | Functional |
| TS_ORD_01 | Order | Verify successful order confirmation | Positive |
| TS_ORD_02 | Order | Verify return to inventory after order completion | Functional |
| TS_ORD_03 | Order | Verify checkout cancellation navigation | Functional |
| TS_ORD_04 | Navigation | Verify logout functionality | Functional |
| TS_ORD_05 | Order | Verify cart state after order completion | Functional |

## Scenario Summary
- Login: 5
- Inventory: 5
- Sorting: 5
- Shopping Cart: 5
- Checkout: 5
- Order Completion and Navigation: 5
- Total: 30

## Testing Status
Test scenario design completed as an initial draft. Detailed test cases and execution results will be documented separately.

## Note
These scenarios were independently designed for portfolio practice. Expected application behavior will be verified during test case preparation and execution.
