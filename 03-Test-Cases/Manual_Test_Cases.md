# SauceDemo — Detailed Manual Test Cases

**Project:** SauceDemo Manual Testing  
**Document ID:** STC-001  
**Version:** 1.0  
**Prepared By:** Pallavi Mogal  
**Status:** Draft — Test Design

## Test Case Summary


| Test Case ID | Scenario ID | Module | Test Case Title | Priority | Status |
|---|---|---|---|---|---|
| TC_LOGIN_001 | TS_LOGIN_01 | Login & Authentication | Verify successful login with valid credentials | High | Not Run |
| TC_LOGIN_002 | TS_LOGIN_02 | Login & Authentication | Verify login with invalid password | High | Not Run |
| TC_LOGIN_003 | TS_LOGIN_03 | Login & Authentication | Verify login with invalid username | High | Not Run |
| TC_LOGIN_004 | TS_LOGIN_04 | Login & Authentication | Verify login with blank username | High | Not Run |
| TC_LOGIN_005 | TS_LOGIN_05 | Login & Authentication | Verify login with blank password | High | Not Run |
| TC_INV_001 | TS_INV_01 | Inventory | Verify available products display | High | Not Run |
| TC_INV_002 | TS_INV_02 | Inventory | Verify product names and prices display | High | Not Run |
| TC_INV_003 | TS_INV_03 | Inventory | Verify navigation to product details | Medium | Not Run |
| TC_INV_004 | TS_INV_04 | Inventory | Verify product images display | Medium | Not Run |
| TC_INV_005 | TS_INV_05 | Inventory | Verify navigation back to inventory | Medium | Not Run |
| TC_SORT_001 | TS_SORT_01 | Sorting | Verify product-name sorting A to Z | Medium | Not Run |
| TC_SORT_002 | TS_SORT_02 | Sorting | Verify product-name sorting Z to A | Medium | Not Run |
| TC_SORT_003 | TS_SORT_03 | Sorting | Verify price sorting low to high | High | Not Run |
| TC_SORT_004 | TS_SORT_04 | Sorting | Verify price sorting high to low | High | Not Run |
| TC_SORT_005 | TS_SORT_05 | Sorting | Verify changing sort selection | Medium | Not Run |
| TC_CART_001 | TS_CART_01 | Shopping Cart | Verify adding one product to cart | High | Not Run |
| TC_CART_002 | TS_CART_02 | Shopping Cart | Verify adding multiple products | High | Not Run |
| TC_CART_003 | TS_CART_03 | Shopping Cart | Verify removing product from cart | High | Not Run |
| TC_CART_004 | TS_CART_04 | Shopping Cart | Verify cart badge updates | High | Not Run |
| TC_CART_005 | TS_CART_05 | Shopping Cart | Verify cart item details and quantities | High | Not Run |
| TC_CHK_001 | TS_CHK_01 | Checkout | Verify checkout with valid information | High | Not Run |
| TC_CHK_002 | TS_CHK_02 | Checkout | Verify blank first-name validation | High | Not Run |
| TC_CHK_003 | TS_CHK_03 | Checkout | Verify blank last-name validation | High | Not Run |
| TC_CHK_004 | TS_CHK_04 | Checkout | Verify blank postal-code validation | High | Not Run |
| TC_CHK_005 | TS_CHK_05 | Checkout | Verify order-summary items and pricing | High | Not Run |
| TC_ORD_001 | TS_ORD_01 | Order Completion & Navigation | Verify successful order confirmation | High | Not Run |
| TC_ORD_002 | TS_ORD_02 | Order Completion & Navigation | Verify return to inventory after order completion | Medium | Not Run |
| TC_ORD_003 | TS_ORD_03 | Order Completion & Navigation | Verify checkout cancellation navigation | Medium | Not Run |
| TC_ORD_004 | TS_ORD_04 | Order Completion & Navigation | Verify logout functionality | High | Not Run |
| TC_ORD_005 | TS_ORD_05 | Order Completion & Navigation | Verify cart state after order completion | Medium | Not Run |

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

## TC_INV_001 — Verify available products display

**Scenario ID:** TS_INV_01  
**Module:** Inventory  
**Priority:** High  
**Test Type:** Functional  

**Preconditions:**
- Open https://www.saucedemo.com/ and log in with standard_user / secret_sauce.
- Inventory page is open.

**Test Data:**
- User: standard_user

**Test Steps:**
1. Observe the inventory page after successful login.
2. Locate the product listing area.
3. Check whether each visible product is presented as an inventory item.

**Expected Result:** The inventory page shows a product list with individually identifiable items.

**Actual Result:** Not recorded  
**Status:** Not Run  
**Evidence:** Not captured

---

## TC_INV_002 — Verify product names and prices display

**Scenario ID:** TS_INV_02  
**Module:** Inventory  
**Priority:** High  
**Test Type:** Functional  

**Preconditions:**
- Open https://www.saucedemo.com/ and log in with standard_user / secret_sauce.
- Inventory page is open.

**Test Data:**
- Products: items currently listed on inventory page

**Test Steps:**
1. Observe at least three product cards.
2. Check that each selected card shows a product name.
3. Check that each selected card shows a price with a currency indicator.

**Expected Result:** Each selected product card displays a readable product name and price.

**Actual Result:** Not recorded  
**Status:** Not Run  
**Evidence:** Not captured

---

## TC_INV_003 — Verify navigation to product details

**Scenario ID:** TS_INV_03  
**Module:** Inventory  
**Priority:** Medium  
**Test Type:** Functional  

**Preconditions:**
- Open https://www.saucedemo.com/ and log in with standard_user / secret_sauce.
- Inventory page is open.

**Test Data:**
- Product: Sauce Labs Backpack (if available)

**Test Steps:**
1. Find the chosen product in the inventory list.
2. Click its product name or image.
3. Observe the destination page and product information.

**Expected Result:** A product-details view opens for the selected item and displays matching product identity and pricing.

**Actual Result:** Not recorded  
**Status:** Not Run  
**Evidence:** Not captured

---

## TC_INV_004 — Verify product images display

**Scenario ID:** TS_INV_04  
**Module:** Inventory  
**Priority:** Medium  
**Test Type:** Functional / UI  

**Preconditions:**
- Open https://www.saucedemo.com/ and log in with standard_user / secret_sauce.
- Inventory page is open.

**Test Data:**
- Products: three items visible on the page

**Test Steps:**
1. Locate images for at least three listed products.
2. Observe whether each image loads.
3. Check for visibly broken or missing images.

**Expected Result:** Product images are displayed without broken-image placeholders for the sampled items.

**Actual Result:** Not recorded  
**Status:** Not Run  
**Evidence:** Not captured

---

## TC_INV_005 — Verify navigation back to inventory

**Scenario ID:** TS_INV_05  
**Module:** Inventory  
**Priority:** Medium  
**Test Type:** Functional / Navigation  

**Preconditions:**
- Open https://www.saucedemo.com/ and log in with standard_user / secret_sauce.
- A product-details page has been opened from inventory.

**Test Data:**
- Product: any available item

**Test Steps:**
1. On the product-details page, locate the Back to products control.
2. Select Back to products.
3. Observe the destination and the visible product list.

**Expected Result:** The inventory list is displayed again after returning from product details.

**Actual Result:** Not recorded  
**Status:** Not Run  
**Evidence:** Not captured

---

## TC_SORT_001 — Verify product-name sorting A to Z

**Scenario ID:** TS_SORT_01  
**Module:** Sorting  
**Priority:** Medium  
**Test Type:** Functional  

**Preconditions:**
- Open https://www.saucedemo.com/ and log in with standard_user / secret_sauce.
- Inventory page with multiple products is open.

**Test Data:**
- Sort option: Name (A to Z)

**Test Steps:**
1. Record the visible product names in their current order.
2. Choose Name (A to Z) from the sort dropdown.
3. Read product names from top to bottom.
4. Compare their order alphabetically.

**Expected Result:** Visible product names are in ascending alphabetical order.

**Actual Result:** Not recorded  
**Status:** Not Run  
**Evidence:** Not captured

---

## TC_SORT_002 — Verify product-name sorting Z to A

**Scenario ID:** TS_SORT_02  
**Module:** Sorting  
**Priority:** Medium  
**Test Type:** Functional  

**Preconditions:**
- Open https://www.saucedemo.com/ and log in with standard_user / secret_sauce.
- Inventory page with multiple products is open.

**Test Data:**
- Sort option: Name (Z to A)

**Test Steps:**
1. Select Name (Z to A) from the sort dropdown.
2. Read product names from top to bottom.
3. Compare their order alphabetically.

**Expected Result:** Visible product names are in descending alphabetical order.

**Actual Result:** Not recorded  
**Status:** Not Run  
**Evidence:** Not captured

---

## TC_SORT_003 — Verify price sorting low to high

**Scenario ID:** TS_SORT_03  
**Module:** Sorting  
**Priority:** High  
**Test Type:** Functional  

**Preconditions:**
- Open https://www.saucedemo.com/ and log in with standard_user / secret_sauce.
- Inventory page with multiple priced products is open.

**Test Data:**
- Sort option: Price (low to high)

**Test Steps:**
1. Select Price (low to high) from the sort dropdown.
2. Record product prices in their displayed order.
3. Compare adjacent price values numerically.

**Expected Result:** Displayed prices follow nondecreasing numeric order from lowest to highest.

**Actual Result:** Not recorded  
**Status:** Not Run  
**Evidence:** Not captured

---

## TC_SORT_004 — Verify price sorting high to low

**Scenario ID:** TS_SORT_04  
**Module:** Sorting  
**Priority:** High  
**Test Type:** Functional  

**Preconditions:**
- Open https://www.saucedemo.com/ and log in with standard_user / secret_sauce.
- Inventory page with multiple priced products is open.

**Test Data:**
- Sort option: Price (high to low)

**Test Steps:**
1. Select Price (high to low) from the sort dropdown.
2. Record product prices in their displayed order.
3. Compare adjacent price values numerically.

**Expected Result:** Displayed prices follow nonincreasing numeric order from highest to lowest.

**Actual Result:** Not recorded  
**Status:** Not Run  
**Evidence:** Not captured

---

## TC_SORT_005 — Verify changing sort selection

**Scenario ID:** TS_SORT_05  
**Module:** Sorting  
**Priority:** Medium  
**Test Type:** Functional  

**Preconditions:**
- Open https://www.saucedemo.com/ and log in with standard_user / secret_sauce.
- Inventory page is open.

**Test Data:**
- First: Name (A to Z)
- Second: Price (high to low)

**Test Steps:**
1. Select Name (A to Z) and observe the product order.
2. Change the selection to Price (high to low).
3. Check the selected option shown in the dropdown.
4. Compare displayed prices from top to bottom.

**Expected Result:** The newly selected option is shown, and the products are reordered according to descending price.

**Actual Result:** Not recorded  
**Status:** Not Run  
**Evidence:** Not captured

---

## TC_CART_001 — Verify adding one product to cart

**Scenario ID:** TS_CART_01  
**Module:** Shopping Cart  
**Priority:** High  
**Test Type:** Positive / Functional  

**Preconditions:**
- Open https://www.saucedemo.com/ and log in with standard_user / secret_sauce.
- Reset application state if prior cart contents may interfere.
- Inventory page is open.

**Test Data:**
- Product: Sauce Labs Backpack (if available)

**Test Steps:**
1. Select Add to cart for the chosen product.
2. Observe the button state and shopping-cart badge.
3. Open the shopping cart.
4. Find the selected product in the cart.

**Expected Result:** The selected product is shown in the cart, and the badge reflects one item when the cart was initially empty.

**Actual Result:** Not recorded  
**Status:** Not Run  
**Evidence:** Not captured

---

## TC_CART_002 — Verify adding multiple products

**Scenario ID:** TS_CART_02  
**Module:** Shopping Cart  
**Priority:** High  
**Test Type:** Positive / Functional  

**Preconditions:**
- Open https://www.saucedemo.com/ and log in with standard_user / secret_sauce.
- Start with an empty cart.

**Test Data:**
- Products: two distinct products from inventory

**Test Steps:**
1. Click Add to cart for the first product.
2. Click Add to cart for the second product.
3. Open the cart.
4. Inspect listed product names and the cart badge.

**Expected Result:** Both selected products appear as separate cart line items, and the cart badge reflects two items.

**Actual Result:** Not recorded  
**Status:** Not Run  
**Evidence:** Not captured

---

## TC_CART_003 — Verify removing product from cart

**Scenario ID:** TS_CART_03  
**Module:** Shopping Cart  
**Priority:** High  
**Test Type:** Functional  

**Preconditions:**
- Open https://www.saucedemo.com/ and log in with standard_user / secret_sauce.
- At least one product is already in the cart.

**Test Data:**
- Product: any item currently in cart

**Test Steps:**
1. Open the cart.
2. Identify a product and select Remove for it.
3. Inspect the remaining cart items and shopping-cart badge.

**Expected Result:** The removed product no longer appears in the cart, and the badge reflects the remaining item count (or disappears if empty).

**Actual Result:** Not recorded  
**Status:** Not Run  
**Evidence:** Not captured

---

## TC_CART_004 — Verify cart badge updates

**Scenario ID:** TS_CART_04  
**Module:** Shopping Cart  
**Priority:** High  
**Test Type:** Functional / State  

**Preconditions:**
- Open https://www.saucedemo.com/ and log in with standard_user / secret_sauce.
- Start with an empty cart.

**Test Data:**
- Products: two distinct products

**Test Steps:**
1. From inventory, add the first product.
2. Record the badge count.
3. Add a second distinct product.
4. Record the badge count.
5. Remove one of the products.
6. Record the updated badge count.

**Expected Result:** The badge reflects 1, then 2, then 1 item across these actions.

**Actual Result:** Not recorded  
**Status:** Not Run  
**Evidence:** Not captured

---

## TC_CART_005 — Verify cart item details and quantities

**Scenario ID:** TS_CART_05  
**Module:** Shopping Cart  
**Priority:** High  
**Test Type:** Functional  

**Preconditions:**
- Open https://www.saucedemo.com/ and log in with standard_user / secret_sauce.
- At least one product has been added to the cart.

**Test Data:**
- Product: record name and price from inventory

**Test Steps:**
1. Record the selected product name and price in inventory.
2. Open the shopping cart.
3. Compare the cart product name and price with inventory.
4. Inspect the displayed quantity for this product.

**Expected Result:** Cart product identity and price match the selected inventory item; quantity is displayed and reflects the item added under the starting conditions.

**Actual Result:** Not recorded  
**Status:** Not Run  
**Evidence:** Not captured

---

## TC_CHK_001 — Verify checkout with valid information

**Scenario ID:** TS_CHK_01  
**Module:** Checkout  
**Priority:** High  
**Test Type:** Positive / End-to-end  

**Preconditions:**
- Open https://www.saucedemo.com/ and log in with standard_user / secret_sauce.
- At least one item is present in the cart.

**Test Data:**
- First name: Alex
- Last name: Tester
- Postal code: 12345 (fictional test data)

**Test Steps:**
1. Open the cart and select Checkout.
2. Enter the supplied first name, last name, and postal code.
3. Select Continue.
4. Observe the checkout overview page.

**Expected Result:** The supplied information is accepted and the checkout overview is displayed with order items and totals.

**Actual Result:** Not recorded  
**Status:** Not Run  
**Evidence:** Not captured

---

## TC_CHK_002 — Verify blank first-name validation

**Scenario ID:** TS_CHK_02  
**Module:** Checkout  
**Priority:** High  
**Test Type:** Negative / Required field  

**Preconditions:**
- Open https://www.saucedemo.com/ and log in with standard_user / secret_sauce.
- At least one item is in the cart.
- Checkout information page is open.

**Test Data:**
- First name: blank
- Last name: Tester
- Postal code: 12345

**Test Steps:**
1. Leave First Name empty.
2. Enter Tester in Last Name.
3. Enter 12345 in Postal Code.
4. Click Continue.

**Expected Result:** Progress to overview is prevented, and an error indicates First Name is required.

**Actual Result:** Not recorded  
**Status:** Not Run  
**Evidence:** Not captured

---

## TC_CHK_003 — Verify blank last-name validation

**Scenario ID:** TS_CHK_03  
**Module:** Checkout  
**Priority:** High  
**Test Type:** Negative / Required field  

**Preconditions:**
- Open https://www.saucedemo.com/ and log in with standard_user / secret_sauce.
- At least one item is in the cart.
- Checkout information page is open.

**Test Data:**
- First name: Alex
- Last name: blank
- Postal code: 12345

**Test Steps:**
1. Enter Alex in First Name.
2. Leave Last Name empty.
3. Enter 12345 in Postal Code.
4. Click Continue.

**Expected Result:** Progress to overview is prevented, and an error indicates Last Name is required.

**Actual Result:** Not recorded  
**Status:** Not Run  
**Evidence:** Not captured

---

## TC_CHK_004 — Verify blank postal-code validation

**Scenario ID:** TS_CHK_04  
**Module:** Checkout  
**Priority:** High  
**Test Type:** Negative / Required field  

**Preconditions:**
- Open https://www.saucedemo.com/ and log in with standard_user / secret_sauce.
- At least one item is in the cart.
- Checkout information page is open.

**Test Data:**
- First name: Alex
- Last name: Tester
- Postal code: blank

**Test Steps:**
1. Enter Alex in First Name.
2. Enter Tester in Last Name.
3. Leave Postal Code empty.
4. Click Continue.

**Expected Result:** Progress to overview is prevented, and an error indicates Postal Code is required.

**Actual Result:** Not recorded  
**Status:** Not Run  
**Evidence:** Not captured

---

## TC_CHK_005 — Verify order-summary items and pricing

**Scenario ID:** TS_CHK_05  
**Module:** Checkout  
**Priority:** High  
**Test Type:** Functional / Calculation  

**Preconditions:**
- Open https://www.saucedemo.com/ and log in with standard_user / secret_sauce.
- At least one item is in cart.
- Checkout information has been submitted successfully.

**Test Data:**
- Products: record names and prices from cart
- Tax: use displayed tax value (do not assume a fixed rate)

**Test Steps:**
1. On checkout overview, compare item names and prices with the cart.
2. Record the displayed Item total, Tax, and Total.
3. Independently sum the item prices.
4. Calculate Item total + Tax and compare with displayed Total, allowing for displayed currency rounding.

**Expected Result:** Checkout overview contains matching line items; Item total equals the sum of item prices; displayed Total equals Item total plus displayed Tax (subject to currency rounding).

**Actual Result:** Not recorded  
**Status:** Not Run  
**Evidence:** Not captured

---

## TC_ORD_001 — Verify successful order confirmation

**Scenario ID:** TS_ORD_01  
**Module:** Order Completion & Navigation  
**Priority:** High  
**Test Type:** Positive / End-to-end  

**Preconditions:**
- Open https://www.saucedemo.com/ and log in with standard_user / secret_sauce.
- At least one cart item is present.
- Checkout information is valid and the overview is visible.

**Test Data:**
- Customer: fictional test details
- Product: any available inventory item

**Test Steps:**
1. Review the checkout overview.
2. Select Finish.
3. Observe the next page and confirmation message.

**Expected Result:** The order-complete view appears and presents a successful order confirmation.

**Actual Result:** Not recorded  
**Status:** Not Run  
**Evidence:** Not captured

---

## TC_ORD_002 — Verify return to inventory after order completion

**Scenario ID:** TS_ORD_02  
**Module:** Order Completion & Navigation  
**Priority:** Medium  
**Test Type:** Functional / Navigation  

**Preconditions:**
- Open https://www.saucedemo.com/ and log in with standard_user / secret_sauce.
- An order has been completed and confirmation page is open.

**Test Data:**
- No additional test data

**Test Steps:**
1. Locate the Back Home control on the confirmation page.
2. Select Back Home.
3. Observe the resulting page.

**Expected Result:** The user returns to the inventory page and can see the product list.

**Actual Result:** Not recorded  
**Status:** Not Run  
**Evidence:** Not captured

---

## TC_ORD_003 — Verify checkout cancellation navigation

**Scenario ID:** TS_ORD_03  
**Module:** Order Completion & Navigation  
**Priority:** Medium  
**Test Type:** Functional / Navigation  

**Preconditions:**
- Open https://www.saucedemo.com/ and log in with standard_user / secret_sauce.
- At least one item is in cart.
- Checkout information or checkout overview page is open.

**Test Data:**
- Page under test: record whether information or overview

**Test Steps:**
1. Record the current checkout stage.
2. Click Cancel.
3. Observe the destination page.
4. Record whether cart items are retained.

**Expected Result:** Cancel exits the current checkout stage without placing an order; the destination follows the observed navigation behavior, which must be recorded and confirmed during execution.

**Actual Result:** Not recorded  
**Status:** Not Run  
**Evidence:** Not captured

---

## TC_ORD_004 — Verify logout functionality

**Scenario ID:** TS_ORD_04  
**Module:** Order Completion & Navigation  
**Priority:** High  
**Test Type:** Functional / Authentication  

**Preconditions:**
- Open https://www.saucedemo.com/ and log in with standard_user / secret_sauce.
- User is logged into SauceDemo.

**Test Data:**
- User: standard_user

**Test Steps:**
1. Open the application menu.
2. Select Logout.
3. Observe the destination screen.
4. Attempt to use the former authenticated workflow via normal navigation.

**Expected Result:** The user returns to the login screen and the active authenticated session is ended.

**Actual Result:** Not recorded  
**Status:** Not Run  
**Evidence:** Not captured

---

## TC_ORD_005 — Verify cart state after order completion

**Scenario ID:** TS_ORD_05  
**Module:** Order Completion & Navigation  
**Priority:** Medium  
**Test Type:** Functional / State  

**Preconditions:**
- Open https://www.saucedemo.com/ and log in with standard_user / secret_sauce.
- Start with an empty cart.
- At least one item is added and a checkout is completed.

**Test Data:**
- Product: one product selected for the completed order

**Test Steps:**
1. Complete checkout for the selected item.
2. Return to the inventory page using Back Home.
3. Open the shopping cart.
4. Record the displayed items and badge state.

**Expected Result:** The post-order cart state follows the intended application behavior; check whether completed-order items are cleared. If no authoritative requirement exists, document the observed behavior as a baseline rather than automatically filing a defect.

**Actual Result:** Not recorded  
**Status:** Not Run  
**Evidence:** Not captured

---


## Execution Notes

- All cases are currently in Not Run status.
- Actual results and evidence will be recorded during execution.
- Expected behaviors are initial testing expectations and will be reviewed against available requirements.
- No defect has been reported or confirmed at this stage.
