# Test Execution Summary – SauceDemo Web Application

## 1. Test Execution Overview

| Item | Details |
|------|---------|
| Application | SauceDemo Web Application |
| Test Type | Manual Functional & Exploratory Testing |
| Primary Test User | standard_user |
| Exploratory Test User | problem_user |
| Browser | Google Chrome |
| Operating System | Windows 11 |
| Execution Status | In Progress |

---

## 2. Standard User – Functional Testing

The `standard_user` account was used as the baseline account for functional testing.

| Metric | Result |
|--------|--------|
| Planned Test Cases | 40 |
| Executed | 40 |
| Passed | 40 |
| Failed | 0 |
| Blocked | 0 |
| Pass Rate | 100% |

### Result

All 40 functional test cases executed with `standard_user` passed successfully.

---

## 3. Problem User – Exploratory Testing

The `problem_user` account was tested to identify user-specific functional and UI issues.

### Confirmed Defects

| Bug ID | Module | Defect | Severity | Priority |
|--------|--------|--------|----------|----------|
| BUG-001 | Product Listing | All products display the same dog image | Medium | Medium |
| BUG-002 | Product Details | Backpack opens Fleece Jacket details | High | High |
| BUG-003 | Product Details | Add to Cart does not work | Medium | Medium |
| BUG-004 | Shopping Cart | Cart badge count does not match cart contents | Medium | Medium |
| BUG-005 | Product Details | Fleece Jacket opens ITEM NOT FOUND page | High | High |
| BUG-006 | Product Details | Remove button does not work | Medium | Medium |
| BUG-007 | Checkout | Last Name input is redirected to First Name field | High | High |

### Exploratory Testing Result

Seven functional/UI defects were identified while testing `problem_user`.

All confirmed defects have been documented separately in the `bug-reports` directory.

---

## 4. Current Testing Status

### Completed

- Standard user functional testing
- Login testing
- Product Listing testing
- Product Details testing
- Shopping Cart testing
- Checkout testing
- Order completion testing
- Order PDF generation testing
- Problem user exploratory testing

### Pending

The following SauceDemo purpose-built users remain to be tested:

- `locked_out_user`
- `performance_glitch_user`
- `error_user`
- `visual_user`

---

## 5. Current Conclusion

The baseline functional testing using `standard_user` was completed successfully with a 100% pass rate.

Exploratory testing using `problem_user` identified seven confirmed defects affecting product display, product navigation, cart functionality, and checkout.

Testing is still in progress because the remaining purpose-built SauceDemo users have not yet been evaluated.
