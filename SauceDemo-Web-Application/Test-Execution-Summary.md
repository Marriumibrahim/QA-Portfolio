# Test Execution Summary – SauceDemo Web Application

## 1. Document Information

| Item | Details |
|------|---------|
| Project | SauceDemo Web Application |
| Application | SauceDemo |
| Test Type | Manual Functional, Exploratory & Visual Testing |
| Primary Test Account | `standard_user` |
| Additional Test Accounts | `locked_out_user`, `problem_user`, `performance_glitch_user`, `error_user`, `visual_user` |
| Browser | Google Chrome |
| Operating System | Windows 11 |
| Execution Status | Completed |

---

## 2. Test Execution Overview

Testing was performed using the SauceDemo application to validate core functionality and identify user-specific functional, performance, and visual issues.

The `standard_user` account was used as the baseline account for executing the planned functional test cases.

The additional SauceDemo test accounts were then evaluated using targeted exploratory testing to identify account-specific application behavior.

---

## 3. Standard User – Functional Test Execution

The `standard_user` account was used to execute the planned functional test cases covering:

- Login
- Product Listing
- Product Details
- Product Sorting
- Shopping Cart
- Checkout
- Order Completion
- Order Receipt / PDF Generation

| Metric | Result |
|--------|--------:|
| Planned Test Cases | 40 |
| Executed | 40 |
| Passed | 40 |
| Failed | 0 |
| Blocked | 0 |
| Pass Rate | 100% |

### Result

All 40 planned functional test cases executed with `standard_user` passed successfully.

The `standard_user` account was therefore used as the baseline for comparison with the purpose-built SauceDemo accounts.

---

# 4. Purpose-Built User Testing

## 4.1 `locked_out_user`

### Test Objective

Verify the behavior of an account that is intentionally locked out.

### Result

Login was attempted using:

- Username: `locked_out_user`
- Password: `secret_sauce`

### Actual Result

The application displayed:

> "Epic sadface: Sorry, this user has been locked out."

The user was not allowed to log in.

### Status

**Pass**

The observed behavior is consistent with the expected purpose of the locked-out test account.

---

## 4.2 `problem_user`

Targeted exploratory testing was performed using `problem_user`.

### Key Findings

The following defects were identified:

| Bug ID | Module | Defect | Severity | Priority |
|--------|--------|---------|----------|----------|
| BUG-001 | Product Listing | Incorrect product images displayed | Medium | Medium |
| BUG-002 | Product Details | Backpack opens Fleece Jacket details | High | High |
| BUG-003 | Product Details | Add to Cart does not work on Product Details page | Medium | Medium |
| BUG-004 | Shopping Cart | Cart badge count does not match cart contents | Medium | Medium |
| BUG-005 | Product Details | Fleece Jacket opens incorrect ITEM NOT FOUND page | High | High |
| BUG-006 | Product Details | Remove button does not work on Product Details page | Medium | Medium |
| BUG-007 | Checkout | Last Name input is redirected to First Name field | High | High |

### Result

**7 confirmed defects identified.**

---

# 5. `performance_glitch_user`

Targeted functional and performance observations were performed using `performance_glitch_user`.

### Functional Results

| Area | Result |
|------|--------|
| Login | Pass |
| Products Page | Pass |
| Product Selection | Pass |
| Product Details | Pass |
| Add to Cart | Pass |
| Shopping Cart | Pass |

### Performance Observation

A noticeable response delay was observed when:

- Returning to the Products page from Product Details.
- Selecting Continue Shopping from the Shopping Cart.

The actions eventually completed successfully.

### Result

**Functional testing: Pass**

**Performance observation recorded.**

No confirmed performance defect was raised because response times were not formally measured.

---

# 6. `error_user`

Targeted exploratory testing was performed using `error_user`.

### Key Findings

| Area | Observation | Result |
|------|-------------|--------|
| Login | Login successful | Pass |
| Products | Six products displayed | Pass |
| Product Images | Broken image icons displayed | Defect |
| Add to Cart | Product added successfully | Pass |
| Remove | Remove button does not work | Defect |
| Product Details | Product details not displayed correctly | Defect |
| Sorting | Sorting fails and error message is displayed | Defect |
| Last Name | Last Name field does not accept input | Defect |
| Checkout Continue | Checkout proceeds without required Last Name | Defect |
| Finish | Finish button does not complete order | Defect |
| Cancel | Cancel redirects to Products page | Defect |

### Error Message Observed

The sorting functionality displayed:

> "Sorting is broken! This error has been reported to Backtrace."

### Confirmed Defects

| Bug ID | Defect | Severity |
|--------|--------|----------|
| BUG-008 | Last Name field does not accept input | High |
| BUG-009 | Checkout continues without required Last Name | High |

Additional observations were recorded during exploratory testing and should be considered during defect review.

---

# 7. `visual_user`

Visual and UI-focused testing was performed using `visual_user`.

### Confirmed Visual Defects

| Bug ID | Module | Defect | Severity |
|--------|--------|---------|----------|
| BUG-010 | Product Listing | Incorrect/wrong-sized Sauce Labs Backpack image | Medium |
| BUG-011 | Navigation | Cart icon incorrectly positioned across pages | Low |
| BUG-012 | Product Listing | Inconsistent product heading alignment | Low |
| BUG-013 | Product Listing | Test.allTheThings() Add to Cart button overflows product card | Medium |
| BUG-014 | Product Details | Add to Cart button incorrectly positioned | Medium |
| BUG-015 | Shopping Cart | Checkout button incorrectly positioned | Medium |
| BUG-016 | Shopping Cart | Quantity and Description columns are merged/misaligned | Medium |

### Additional Visual Checks

The following areas were checked and no additional visual issues were observed:

- Checkout Overview
- Payment Information
- Shipping Information
- Price Summary
- Finish button
- Checkout Complete page
- Back Home button
- Generate PDF Order button

### Result

**7 visual defects identified.**

---

# 8. Defect Summary

The current defect log contains **16 documented defects**.

| Severity | Number of Defects |
|----------|------------------:|
| High | 5 |
| Medium | 9 |
| Low | 2 |
| **Total** | **16** |

### Severity Distribution

- **High:** BUG-002, BUG-005, BUG-007, BUG-008, BUG-009
- **Medium:** BUG-001, BUG-003, BUG-004, BUG-006, BUG-010, BUG-013, BUG-014, BUG-015, BUG-016
- **Low:** BUG-011, BUG-012

> Note: Severity should be reviewed again during formal defect triage if additional business-impact information becomes available.

---

# 9. Overall Test Status

| Test Area | Status |
|-----------|--------|
| Standard User Functional Testing | Completed |
| Locked-Out User Testing | Completed |
| Problem User Exploratory Testing | Completed |
| Performance Glitch User Testing | Completed |
| Error User Exploratory Testing | Completed |
| Visual User Testing | Completed |
| Defect Documentation | Completed |
| Regression Testing | Pending |

---

# 10. Overall Conclusion

The planned baseline functional testing using `standard_user` was completed with all 40 test cases passing.

Targeted exploratory testing of the SauceDemo purpose-built accounts identified multiple functional, UI, and user-specific defects.

A total of 16 defects have been documented:

- 5 High severity
- 9 Medium severity
- 2 Low severity

The most significant issues affect product navigation, checkout functionality, product information, and cart behavior.

The application demonstrates successful baseline functionality for `standard_user`, but the identified defects require investigation and retesting before considering the application fully stable across all supported user scenarios.

Regression testing should be performed after the identified defects are fixed.
