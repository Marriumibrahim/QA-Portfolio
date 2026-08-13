# SauceDemo – Software Quality Assurance Project

Manual Software Quality Assurance testing project for the SauceDemo e-commerce web application.

This project demonstrates practical QA activities including functional testing, test case design, exploratory testing, visual testing, defect reporting, test execution, and test summary reporting.

---

## Project Overview

**Application:** SauceDemo E-Commerce Web Application

**Testing Type:**
- Manual Functional Testing
- Exploratory Testing
- Visual/UI Testing
- Regression Testing
- User-Specific Testing

**Primary Test User:** `standard_user`

**Additional Test Users:**
- `locked_out_user`
- `problem_user`
- `performance_glitch_user`
- `error_user`
- `visual_user`

**Browser:** Google Chrome

**Operating System:** Windows 11

---

## Testing Objectives

The objective of this project was to validate the core functionality and user experience of the SauceDemo application.

Testing focused on:

- User authentication
- Product listing
- Product sorting
- Product details
- Add to Cart functionality
- Shopping Cart
- Remove from Cart
- Checkout
- Order completion
- Order receipt / PDF generation
- User-specific application behavior
- Visual/UI consistency

---

## Test Coverage

The following application areas were covered:

| Module | Coverage |
|---|---|
| Login | Valid and invalid login behavior |
| Products | Product listing and product information |
| Sorting | Product sorting functionality |
| Product Details | Product navigation and information |
| Shopping Cart | Add, remove, quantity and cart count |
| Checkout | Customer information and validation |
| Order Completion | Order submission and confirmation |
| Order Receipt | Order details and PDF generation |
| Exploratory Testing | Purpose-built user accounts |
| Visual Testing | UI layout, alignment and positioning |

---

## Test Execution

The `standard_user` account was used as the baseline account for the planned functional test cases.

| Metric | Result |
|---|---:|
| Planned Test Cases | 40 |
| Executed | 40 |
| Passed | 40 |
| Failed | 0 |
| Blocked | 0 |
| Pass Rate | **100%** |

Additional exploratory testing was performed using SauceDemo's purpose-built user accounts.

---

## Purpose-Built User Testing

| User | Testing Focus | Result |
|---|---|---|
| `standard_user` | Functional Testing | 40/40 Passed |
| `locked_out_user` | Authentication | Expected lockout behavior |
| `problem_user` | Exploratory Testing | 7 defects identified |
| `performance_glitch_user` | Functional / Performance Observation | Functional flow passed |
| `error_user` | Exploratory Testing | 2 documented defects |
| `visual_user` | Visual/UI Testing | 7 visual defects identified |

---

## Defect Summary

A total of **16 defects** were documented during testing.

| Severity | Count |
|---|---:|
|  High | 5 |
|  Medium | 9 |
|  Low | 2 |
| **Total** | **16** |

### Defect Distribution

| User | Defects |
|---|---:|
| `problem_user` | 7 |
| `error_user` | 2 |
| `visual_user` | 7 |
| **Total** | **16** |

---

## Key Findings

The baseline functional testing using `standard_user` achieved a **100% pass rate**.

Exploratory testing of purpose-built users identified issues affecting:

- Product navigation
- Product information
- Shopping Cart behavior
- Checkout validation
- Product images
- UI alignment
- Button positioning
- Cart layout

A noticeable performance delay was also observed with `performance_glitch_user` during some navigation actions. This was recorded as a performance observation because formal response-time measurements were not performed.

---

## QA Assessment

### Not Ready for Release

Although all 40 baseline functional test cases passed with `standard_user`, **16 defects** were identified during additional exploratory and visual testing.

The presence of **5 High severity defects** means the application should not currently be considered ready for release.

Recommended next steps:

1. Fix High severity defects.
2. Retest affected functionality.
3. Execute regression testing.
4. Verify that fixes do not introduce new defects.
5. Perform additional cross-browser and performance testing before release.

---

## Project Artifacts

### Test Documentation

- [Test Plan](test-plan.md)
- [Test Scenarios](test-scenarios.md)
- [Test Cases](test-cases.md)
- [Test Execution Summary](test-execution-summary.md)
- [Test Summary Report](test-summary-report.md)

### Bug Reports

All documented defects are available in the [`bug-reports`](bug-reports/) directory.

- BUG-001 – BUG-016
- 16 documented defects
- High, Medium and Low severity classifications

---

## Testing Approach

The project followed a practical QA workflow:

```text
Requirement Understanding
        ↓
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
