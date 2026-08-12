# Test Execution Summary – SauceDemo Web Application

## Document Information

| Item | Details |
|------|---------|
| Project | SauceDemo Web Application |
| Application | SauceDemo Web Application |
| Test Type | Manual Functional Testing |
| Primary Test User | standard_user |
| Additional Test User | problem_user |
| Environment | Windows 11 / Google Chrome |
| Execution Status | In Progress |

---

## 1. Standard User Test Execution Summary

The initial functional test execution was performed using the SauceDemo `standard_user` account.

| Module | Test Cases Executed | Passed | Failed | Blocked |
|--------|--------------------:|-------:|-------:|--------:|
| Login | 8 | 8 | 0 | 0 |
| Product Listing |  |  |  |  |
| Product Details |  |  |  |  |
| Shopping Cart |  |  |  |  |
| Checkout |  |  |  |  |
| **Total** | **40** | **40** | **0** | **0** |

### Standard User Result

All executed test cases for `standard_user` passed successfully.

The `standard_user` account was used as the baseline for comparison with the purpose-built SauceDemo test accounts.

---

## 2. User-Specific / Exploratory Testing

Additional exploratory testing was performed using the SauceDemo `problem_user` account.

The purpose was to identify functional and UI issues that may not be present when using `standard_user`.

### Confirmed Defects

| Bug ID | Module | Summary | Severity | Priority | Status |
|--------|--------|---------|----------|----------|--------|
| BUG-001 | Product Listing | All products display the same dog image | Medium | Medium | New |
| BUG-002 | Product Details | Clicking Sauce Labs Backpack opens Sauce Labs Fleece Jacket details | High | High | New |
| BUG-003 | Product Details | Add to Cart does not work on Product Details page | Medium | Medium | New |
| BUG-004 | Shopping Cart | Cart badge count does not match cart contents | Medium | Medium | New |
| BUG-005 | Product Details | Fleece Jacket opens incorrect ITEM NOT FOUND page | High | High | New |
| BUG-006 | Product Details | Remove button does not remove product | Medium | Medium | New |
| BUG-007 | Checkout | Last Name input is redirected to First Name field and characters replace previous input | High | High | New |

---

## 3. Exploratory Testing Observations

The following observations were recorded during testing with `problem_user`:

- Product images were incorrect across the Products page.
- Product navigation displayed incorrect product information.
- Product Details Add to Cart functionality was not working.
- Shopping Cart badge count became inconsistent with the actual cart contents.
- Incorrect Product Details content was displayed for Sauce Labs Fleece Jacket.
- Remove functionality did not work on the Product Details page.
- Checkout Last Name input behaved incorrectly and prevented checkout completion.

Each confirmed defect has been documented separately in the `bug-reports` folder.

---

## 4. Current Execution Status

Standard user functional testing has been completed.

Additional user-specific exploratory testing is currently in progress.

Testing of the remaining SauceDemo purpose-built accounts will be performed separately:

- `locked_out_user`
- `performance_glitch_user`
- `error_user`
- `visual_user`

The final execution summary will be updated after testing of the additional accounts is completed.

---

## 5. Conclusion

The initial functional testing using `standard_user` was completed successfully, with all executed test cases passing.

Additional exploratory testing using `problem_user` identified multiple functional and UI defects. These defects have been documented separately and will be included in the final test summary.

Further testing is required before the overall testing activity can be considered complete.
