# Test Execution Summary – SauceDemo Web Application

## 1. Document Information

| Item | Details |
|------|---------|
| Project | SauceDemo Web Application |
| Application | SauceDemo |
| Test Type | Manual Functional, Exploratory & Visual Testing |
| Primary Test User | `standard_user` |
| Additional Test Users | `locked_out_user`, `problem_user`, `performance_glitch_user`, `error_user`, `visual_user` |
| Browser | Google Chrome |
| Operating System | Windows 11 |
| Execution Status | Completed |

---

## 2. Test Execution Overview

Testing was performed on the SauceDemo web application to validate core functionality and identify user-specific functional, performance, and visual issues.

The `standard_user` account was used as the baseline account for executing the planned functional test cases.

The additional purpose-built SauceDemo accounts were tested separately using targeted exploratory testing.

---

## 3. Standard User – Functional Testing

The `standard_user` account was used to execute the planned functional test cases covering:

- Login
- Product Listing
- Product Sorting
- Product Details
- Shopping Cart
- Checkout
- Order Completion
- Order Receipt / PDF Generation

| Metric | Result |
|--------|-------:|
| Planned Test Cases | 40 |
| Executed | 40 |
| Passed | 40 |
| Failed | 0 |
| Blocked | 0 |
| Pass Rate | 100% |

### Result

All 40 planned functional test cases executed with `standard_user` passed successfully.

---

# 4. Purpose-Built User Testing

## 4.1 `locked_out_user`

### Objective

Verify that a locked-out user cannot access the application.

### Result

Login was attempted using:

- Username: `locked_out_user`
- Password: `secret_sauce`

The application displayed:

> "Epic sadface: Sorry, this user has been locked out."

The user was not allowed to log in.

### Status

**Pass**

---

## 4.2 `problem_user`

Targeted exploratory testing was performed using `problem_user`.

### Confirmed Defects

| Bug ID | Module | Defect | Severity |
|--------|--------|---------|----------|
| BUG-001 | Product Listing | All products display the same dog image | Medium |
| BUG-002 | Product Details | Sauce Labs Backpack opens Sauce Labs Fleece Jacket details | High |
| BUG-003 | Product Details | Add to Cart does not work on Product Details page | Medium |
| BUG-004 | Shopping Cart | Cart badge count does not match cart contents | Medium |
| BUG-005 | Product Details | Sauce Labs Fleece Jacket opens incorrect ITEM NOT FOUND page | High |
| BUG-006 | Product Details | Remove button does not remove product | Medium |
| BUG-007 | Checkout | Last Name input is redirected to First Name field | High |

### Result

**7 confirmed defects identified.**

---

## 4.3 `performance_glitch_user`

Targeted functional and performance testing was performed using `performance_glitch_user`.

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

A noticeable delay was observed when:

- Returning to the Products page from Product Details.
- Selecting Continue Shopping from the Shopping Cart.

The actions eventually completed successfully.

### Result

**Functional testing passed.**

A performance observation was recorded. No confirmed performance defect was raised because response times were not formally measured.

---

## 4.4 `error_user`

Targeted exploratory testing was performed using `error_user`.

### Key Observations

| Area | Result |
|------|--------|
| Login | Pass |
| Products Page | 6 products displayed |
| Product Images | Broken image icons observed |
| Add to Cart | Pass |
| Remove | Failed |
| Product Details | Incorrect product information observed |
| Sorting | Failed with application error message |
| Last Name | Unable to enter Last Name |
| Continue | Checkout proceeded without Last Name |
| Finish | No response |
| Cancel | Redirected to Products page |

### Sorting Error Observed

> "Sorting is broken! This error has been reported to Backtrace."

### Confirmed Defects Documented

| Bug ID | Module | Defect | Severity |
|--------|--------|---------|----------|
| BUG-008 | Checkout | Last Name field does not accept input | High |
| BUG-009 | Checkout | Checkout continues without required Last Name | High |

### Result

**2 defects documented as separate bug reports.**

Other observations were recorded during exploratory testing but were not assigned separate bug IDs in the current defect log.

---

## 4.5 `visual_user`

Visual and UI-focused testing was performed using `visual_user`.

### Confirmed Visual Defects

| Bug ID | Module | Defect | Severity |
|--------|--------|---------|----------|
| BUG-010 | Product Listing | Incorrect product image displayed for Sauce Labs Backpack | Medium |
| BUG-011 | Navigation | Cart icon incorrectly positioned across pages | Low |
| BUG-012 | Product Listing | Product headings have inconsistent alignment | Low |
| BUG-013 | Product Listing | Test.allTheThings() Add to Cart button overflows product card | Medium |
| BUG-014 | Product Details | Add to Cart button incorrectly positioned | Medium |
| BUG-015 | Shopping Cart | Checkout button incorrectly positioned | Medium |
| BUG-016 | Shopping Cart | Quantity and Description columns are merged/misaligned | Medium |

### Additional Visual Checks

The following areas were checked without identifying additional visual defects:

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

# 5. Defect Summary

A total of **16 defects** have been documented in the bug reports.

| Severity | Number of Defects |
|----------|------------------:|
| High | 5 |
| Medium | 9 |
| Low | 2 |
| **Total** | **16** |

### High Severity

- BUG-002
- BUG-005
- BUG-007
- BUG-008
- BUG-009

### Medium Severity

- BUG-001
- BUG-003
- BUG-004
- BUG-006
- BUG-010
- BUG-013
- BUG-014
- BUG-015
- BUG-016

### Low Severity

- BUG-011
- BUG-012

---

# 6. Defect Distribution by User

| User | Documented Defects |
|------|-------------------:|
| `problem_user` | 7 |
| `error_user` | 2 |
| `visual_user` | 7 |
| `locked_out_user` | 0 |
| `performance_glitch_user` | 0 |
| **Total** | **16** |

---

# 7. Overall Testing Status

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

# 8. Overall Conclusion

The planned baseline functional testing using `standard_user` was completed successfully, with all 40 planned test cases passing.

Targeted exploratory testing of the purpose-built SauceDemo users identified functional and visual issues that were not observed during the baseline `standard_user` execution.

A total of **16 defects** have been documented:

- **5 High severity**
- **9 Medium severity**
- **2 Low severity**

The most significant issues affect product navigation, product information, checkout validation, and shopping cart functionality.

The application demonstrated successful baseline functionality for `standard_user`; however, the documented defects require investigation and retesting before the application can be considered fully stable across the tested user scenarios.

Regression testing should be performed after defect fixes are implemented.
