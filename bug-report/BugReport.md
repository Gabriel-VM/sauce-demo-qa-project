# 🐞 Bug Report – Sauce Demo QA Project

Below you have the list of bugs found during manual and exploratory testing of [Sauce Demo](https://www.saucedemo.com/) with a `problem_user` account (except for BUG-010).
You can also view the .pdf document for clarifications [BugReport](./Bug_report.pdf)

---

## 🔹 [BUG-001] [Homepage] [Hamburger Menu] → “About” CTA does not redirect correctly
- **Priority:** Medium
- **Description:** Clicking the “About” option in the hamburger menu redirects to a 404 error page.
- **Steps to Reproduce:**
  1. Login as `problem_user`
  2. Navigate to the Homepage
  3. Open hamburger menu
  4. Click on "About"
- **Actual Result:** Redirects to 404 page
- **Expected Result:** Should redirect to the About page

---

## 🔹 [BUG-002] [Homepage] [Hamburger Menu] → “Reset App State” CTA not working
- **Priority:** High
- **Description:** Clicking "Reset App State" does not reset the application state.
- **Steps to Reproduce:**
  1. Login as `problem_user`
  2. Open hamburger menu
  3. Click on "Reset App State"
- **Actual Result:** App state remains unchanged
- **Expected Result:** App should reset to its initial state (e.g., item counters, cart empty)

---

## 🔹 [BUG-003] [Homepage] [Sorting Selector] → Sorting options don't work
- **Priority:** High
- **Description:** Selecting any sort method does not affect the product display order.
- **Steps to Reproduce:**
  1. Login as `problem_user`
  2. Click on sorting dropdown
  3. Select a sorting method
- **Actual Result:** Products remain unsorted
- **Expected Result:** Products should be reordered based on the selected sorting method

---

## 🔹 [BUG-004] [Homepage] [Item Cards] → All item cards show the same incorrect image
- **Priority:** Highest
- **Description:** All products display the same unrelated image.
- **Steps to Reproduce:**
  1. Login as `problem_user`
  2. View product cards
- **Actual Result:** Same image shown for all products
- **Expected Result:** Each product card should show its corresponding image

---

## 🔹 [BUG-005] [Homepage] [Add to Cart CTA] → Some products are not added
- **Priority:** Highest
- **Affected Products:**
  - Sauce Labs Bolt T-Shirt
  - Sauce Labs Fleece Jacket
  - Test.allTheThings() T-Shirt (Red)
- **Steps to Reproduce:**
  1. Login as `problem_user`
  2. Try adding listed products to cart
- **Actual Result:** Nothing happens; button state doesn't change
- **Expected Result:** Items should be added, button should switch to "Remove"

---

## 🔹 [BUG-006] [Homepage] [Remove CTA] → Unable to remove items from cart
- **Priority:** Highest
- **Description:** Remove button is not clickable
- **Steps to Reproduce:**
  1. Login as `problem_user`
  2. Add item to cart
  3. Click "Remove"
- **Actual Result:** Nothing happens; item stays in cart
- **Expected Result:** Item should be removed and button should revert to "Add to cart"

---

## 🔹 [BUG-007] [Item Details Page] → Page does not match clicked item
- **Priority:** Highest
- **Description:** Clicking a product title leads to the wrong product detail page
- **Steps to Reproduce:**
  1. Login as `problem_user`
  2. Click on a product title
- **Actual Result:** Redirected to incorrect item detail page
- **Expected Result:** Should match selected product

---

## 🔹 [BUG-008] [Item Details Page] [Add to Cart] → Button not clickable
- **Priority:** High
- **Description:** Add to cart button is unresponsive
- **Steps to Reproduce:**
  1. Login as `problem_user`
  2. Open product detail page
  3. Click "Add to cart"
- **Actual Result:** No response
- **Expected Result:** Product added to cart

---

## 🔹 [BUG-009] [Checkout – Personal Info] → Last Name field not fillable
- **Priority:** Highest (Blocking issue)
- **Description:** Typing in the "Last Name" field populates the "First Name" instead
- **Steps to Reproduce:**
  1. Login as `problem_user`
  2. Navigate to Checkout – Step 1
  3. Type in the "Last Name" field
- **Actual Result:** Text appears in the wrong field
- **Expected Result:** Fields should function independently

---

## 🔹 [BUG-010] [Session / Cookies] → Cart data shared between users
- **Priority:** Highest
- **Affected Users:** `problem_user`, `standard_user`
- **Description:** Cart contents persist across different user sessions
- **Steps to Reproduce:**
  1. Login as `problem_user`, add items to cart
  2. Logout
  3. Login as `standard_user`
- **Actual Result:** Items from `problem_user` are visible in `standard_user`'s cart
- **Expected Result:** Sessions and carts should be isolated between users

---
