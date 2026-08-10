# Test Plan – SauceDemo Web Application

## Document Information

| Item | Details |
|------|---------|
| Project | SauceDemo Web Application |
| Application Type | Web Application |
| Document | Test Plan |
| Version | 1.0 |
| Prepared By | Marrium Ibrahim |
| Date | August 2026 |
| Document Status | Draft |

## Project Overview

SauceDemo is a web-based e-commerce application that allows users to log in, browse products, view product details, add and remove products from the shopping cart, proceed through the checkout process, and complete an order.

This test plan defines the testing approach, scope, objectives, test activities, and deliverables for validating the application's core functionality and user workflows.

## Test Objectives

The primary objectives of testing are to:

- Verify that users can successfully log in using valid credentials.
- Verify that products are displayed correctly and can be sorted as expected.
- Verify that users can view product details.
- Verify that products can be added to and removed from the shopping cart.
- Verify that checkout information is validated correctly.
- Verify that order information and totals are displayed correctly.
- Verify that users can successfully complete an order.
- Identify and document defects with clear reproduction steps.
- Verify fixes through retesting and regression testing.
- Ensure critical user workflows remain functional after changes.

## Scope of Testing

### In Scope

- Login
- Product Listing
- Product Sorting
- Product Details
- Shopping Cart
- Checkout
- Order Completion and Confirmation

### Out of Scope

- Security Testing
- Performance Testing

## Test Approach

Testing will primarily be performed using manual black-box testing techniques.

  The following testing activities will be performed:

- Functional Testing
- Smoke Testing
- Sanity Testing
- Regression Testing
- Exploratory Testing
- Retesting of Fixed Defects
- Defect Verification

## Test Environment

| Item | Details |
|------|---------|
| Application | SauceDemo Web Application |
| Application Type | Web Application |
| Operating System | Windows 11 |
| Browser | Google Chrome |
| Testing Type | Manual Testing |
| Test Data | SauceDemo-provided test accounts and test data |

## Entry Criteria

Testing will begin when:

- The test environment is available and accessible.
- The application is accessible and functioning.
- Required test credentials are available.
- The application features included in the testing scope are available for testing.

## Exit Criteria

Testing will be considered complete when:

- All features included in the testing scope have been tested.
- All identified defects have been documented and reported.
- Retesting of fixed defects has been completed where applicable.
- Regression testing has been completed for affected areas.
- No critical functionality remains blocked from testing.

## Test Deliverables

The following QA deliverables will be produced as part of this testing project:

- Test Plan
- Test Scenarios
- Test Cases
- Regression Test Checklist
- Exploratory Testing Notes
- Bug Reports
- Test Execution Results
- Test Summary Report

## Risks and Assumptions

### Risks

- Changes to the publicly available application may affect previously created test cases.
- Temporary application unavailability may interrupt testing.
- Changes in application behavior may require updates to the testing scope and test cases.
- Limited control over the public test environment may affect test execution.

### Assumptions

- The SauceDemo application remains accessible during testing.
- Required test credentials are available.
- The features included in the test scope are functional enough to execute testing.
- Testing will be performed using the documented test environment.
