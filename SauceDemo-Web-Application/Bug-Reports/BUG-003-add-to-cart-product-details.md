# BUG-003 — Add to Cart Does Not Work on Product Details Page

## Summary

When logged in as `problem_user`, the Add to Cart button does not work on the Product Details page.

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
5. Click the **Add to Cart** button.
6. Observe the button and cart badge.

## Expected Result

The Add to Cart button should add the product to the Shopping Cart, change to **Remove**, and update the cart badge.

## Actual Result

The Add to Cart button does not add the product to the Shopping Cart. The button does not change to **Remove**, and the cart badge is not updated.

## Severity

Medium

## Priority

Medium

## Status

New
