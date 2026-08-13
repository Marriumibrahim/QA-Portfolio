# BUG-015 — Checkout Button Incorrectly Positioned

## Summary

When logged in as `visual_user`, the Checkout button is incorrectly positioned at the top-right of the Shopping Cart page.

## Environment

| Item | Details |
|------|---------|
| Application | SauceDemo Web Application |
| User | visual_user |
| Browser | Google Chrome |
| Operating System | Windows 11 |
| Test Type | Visual / UI Testing |

## Preconditions

- SauceDemo application is accessible.
- User is logged in as `visual_user`.
- At least one product has been added to the Shopping Cart.

## Steps to Reproduce

1. Log in using `visual_user`.
2. Add a product to the Shopping Cart.
3. Open the Shopping Cart.
4. Observe the position of the Checkout button.

## Expected Result

The Checkout button should be positioned consistently within the Shopping Cart page layout according to the application's standard design.

## Actual Result

The Checkout button is incorrectly positioned at the top-right of the Shopping Cart page.

## Severity

Medium

## Priority

Medium

## Status

New
