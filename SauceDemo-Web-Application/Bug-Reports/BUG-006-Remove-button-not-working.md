# BUG-006 — Remove Button Does Not Remove Product on Product Details Page

## Summary

When logged in as `problem_user`, clicking the Remove button on the Product Details page does not remove the product from the Shopping Cart.

## Environment

| Item | Details |
|------|---------|
| Application | SauceDemo Web Application |
| User | problem_user |
| Browser | Google Chrome |
| Operating System | Windows 11 |
| Test Type | Functional / Exploratory Testing |

## Preconditions

- SauceDemo application is accessible.
- User is logged in as `problem_user`.
- A product has been added to the Shopping Cart.
- The product's Product Details page is accessible.

## Steps to Reproduce

1. Log in using `problem_user`.
2. Add a product to the Shopping Cart.
3. Open the product's Product Details page.
4. Verify that the Remove button is displayed.
5. Click the Remove button.
6. Observe the Product Details page and Shopping Cart.

## Expected Result

The selected product should be removed from the Shopping Cart.

The Remove button should change back to an Add to Cart button, and the cart count should be updated accordingly.

## Actual Result

Clicking the Remove button produces no visible change.

The product remains in the Shopping Cart.

## Severity

Medium

## Priority

Medium

## Status

New
