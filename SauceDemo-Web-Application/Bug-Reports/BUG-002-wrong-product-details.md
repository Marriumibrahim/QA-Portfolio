# BUG-002 — Clicking a Product Opens Incorrect Product Details

## Summary

When logged in as `problem_user`, clicking a product opens the Product Details page for a different product.

## Environment

| Item | Details |
|------|---------|
| Application | SauceDemo Web Application |
| User | problem_user |
| Browser | Google Chrome |
| Operating System | Windows 11 |
| Test Type | Functional Testing |

## Preconditions

- SauceDemo application is accessible.
- User is logged in as `problem_user`.
- Products page is displayed.

## Steps to Reproduce

1. Log in using `problem_user`.
2. Navigate to the Products page.
3. Click **Sauce Labs Backpack**.
4. Observe the Product Details page.

## Expected Result

The Product Details page for **Sauce Labs Backpack** should be displayed.

## Actual Result

Clicking **Sauce Labs Backpack** opens the Product Details page for **Sauce Labs Fleece Jacket**.
## Severity

High

## Priority

High

## Status

New
