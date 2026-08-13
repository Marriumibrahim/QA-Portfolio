# SauceDemo – Manual QA Testing Project

## Project Overview

This project demonstrates manual Software Quality Assurance testing of the SauceDemo e-commerce web application.

The project covers functional testing, exploratory testing, visual/UI testing, test execution, defect reporting, and test summary reporting.

---

## Application Under Test

**Application:** SauceDemo E-Commerce Web Application

**Primary Test User:** `standard_user`

**Additional Test Users:**

- `locked_out_user`
- `problem_user`
- `performance_glitch_user`
- `error_user`
- `visual_user`

---

## Testing Environment

| Item | Details |
|------|---------|
| Browser | Google Chrome |
| Operating System | Windows 11 |
| Testing Type | Manual Testing |
| Application | SauceDemo |

---

## Testing Objectives

The objective of this project was to verify the functionality and user experience of the SauceDemo application.

Testing covered:

- User Login
- Product Listing
- Product Sorting
- Product Details
- Add to Cart
- Remove from Cart
- Shopping Cart
- Checkout
- Order Completion
- Order Receipt / PDF Generation
- User-Specific Behavior
- Visual/UI Consistency

---

## Test Coverage

| Module | Testing Coverage |
|--------|------------------|
| Login | Login and authentication behavior |
| Products | Product listing, names, images and prices |
| Sorting | Product sorting functionality |
| Product Details | Product navigation and information |
| Shopping Cart | Add, remove, cart count and product information |
| Checkout | Customer information and validation |
| Order Completion | Order submission and confirmation |
| Order Receipt | Order details and PDF generation |
| Exploratory Testing | Purpose-built SauceDemo users |
| Visual Testing | Layout, alignment and positioning |

---

## Test Execution Summary

The `standard_user` account was used as the baseline account for the planned functional test cases.

| Metric | Result |
|--------|--------:|
| Planned Test Cases | 40 |
| Executed | 40 |
| Passed | 40 |
| Failed | 0 |
| Blocked | 0 |
| Pass Rate | **100%** |

All 40 planned functional test cases passed successfully using `standard_user`.

---

## Purpose-Built User Testing

Additional testing was performed using the purpose-built SauceDemo accounts.

| User | Testing Focus | Result |
|------|---------------|--------|
| `standard_user` | Functional Testing | 40/40 Passed |
| `locked_out_user` | Authentication | Expected lockout behavior |
| `problem_user` | Exploratory Testing | 7 defects identified |
| `performance_glitch_user` | Functional / Performance Observation | Functional flow passed |
| `error_user` | Exploratory Testing | 2 documented defects |
| `visual_user` | Visual/UI Testing | 7 visual defects identified |

---

## Defect Summary

A total of **16 defects** were documented during testing.

| Severity | Number of Defects |
|----------|------------------:|
| High | 5 |
| Medium | 9 |
| Low | 2 |
| **Total** | **16** |

### Defect Distribution

| User | Documented Defects |
|------|-------------------:|
| `problem_user` | 7 |
| `error_user` | 2 |
| `visual_user` | 7 |
| **Total** | **16** |

---

## Key Findings

### Functional Testing

The baseline functional testing performed with `standard_user` achieved a **100% pass rate**.

All 40 planned functional test cases passed.

### Exploratory Testing

Testing the purpose-built SauceDemo users revealed issues that were not observed during the baseline testing.

Defects were identified in areas including:

- Product navigation
- Product information
- Shopping Cart
- Checkout validation
- Product behavior

### Visual Testing

Testing with `visual_user` identified several UI and visual issues involving:

- Product images
- Cart icon positioning
- Product heading alignment
- Add to Cart button positioning
- Checkout button positioning
- Shopping Cart layout

### Performance Observation

`performance_glitch_user` showed noticeable delays during some navigation actions compared with `standard_user`.

This was recorded as a performance observation rather than a confirmed performance defect because formal response-time measurements were not performed.

---

## QA Assessment

### ⚠️ Not Ready for Release

Although the baseline functional testing achieved a **100% pass rate**, additional exploratory and visual testing identified **16 defects**, including **5 High severity defects**.

The application should not be considered ready for release until the High severity defects are fixed and successfully retested.

Regression testing should also be performed after defect fixes.

---

## Project Artifacts

### Test Documentation

- [Test Plan](Test-Plan.md)
- [Test Scenarios](Test-Scenarios.md)
- [Test Cases](Test-Cases.md)
- [Application Study](Application-Study.md)
- [Test Execution Summary](Test-Execution-Summary.md)
- [Test Summary Report](Test-Summary-Report.md)

### Bug Reports

📁 [View all 16 documented bug reports](Bug-Reports/)

The following defects were identified and documented during testing:

1. BUG-001 – Incorrect Product Images
2. BUG-002 – Wrong Product Details
3. BUG-003 – Add to Cart on Product Details
4. BUG-004 – Cart Badge Count Not Updated
5. BUG-005 – Incorrect Product Details / ITEM NOT FOUND
6. BUG-006 – Remove Button Not Working
7. BUG-007 – Last Name Input Entered Into First Name Field
8. BUG-008 – Last Name Field Does Not Accept Input
9. BUG-009 – Checkout Continues Without Last Name
10. BUG-010 – Incorrect Product Image
11. BUG-011 – Cart Icon Incorrectly Positioned
12. BUG-012 – Inconsistent Product Heading Alignment
13. BUG-013 – Add to Cart Button Overflow
14. BUG-014 – Add to Cart Position on Product Details
15. BUG-015 – Checkout Button Incorrect Position
16. BUG-016 – Quantity / Description Column Issue

**Total: 16 documented defects**

---

## Testing Workflow

The project followed this QA workflow:

```text
Test Planning
      ↓
Test Scenario Design
      ↓
Test Case Design
      ↓
Functional Test Execution
      ↓
Exploratory Testing
      ↓
Visual Testing
      ↓
Defect Reporting
      ↓
Test Execution Summary
      ↓
Test Summary Report
      ↓
Regression Testing
---

## Tools Used

- Manual Testing
- GitHub
- Markdown
- Google Chrome
- Windows 11
- SauceDemo
- Test Case Documentation
- Defect Reporting

---

## Project Purpose

This project demonstrates practical Software Quality Assurance skills including:

- Test planning
- Test case design
- Functional testing
- Exploratory testing
- Visual testing
- Defect identification
- Bug reporting
- Test execution reporting
- QA test summary preparation

---

## Disclaimer

This project was created for QA learning and portfolio purposes.

It does not contain confidential, proprietary, or client-owned information.

---

## Author

**Marrium Ibrahim**

Software Quality Assurance Engineer
## Author

**Marrium Ibrahim**

Software Quality Assurance Engineer
