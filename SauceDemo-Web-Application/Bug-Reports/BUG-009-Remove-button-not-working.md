# BUG-009 — Remove Button Does Not Remove Product from Cart on Product Details Page

## Summary

When logged in as `problem_user`, the Remove button on the Product Details page does not remove the selected product from the Shopping Cart.

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
- A product has been added to the Shopping Cart.

## Steps to Reproduce

1. Log in using `problem_user`.
2. Add a product to the Shopping Cart.
3. Open the product's Product Details page.
4. Verify that the Remove button is displayed.
5. Click the Remove button.
6. Observe the button and Shopping Cart.

## Expected Result

The product should be removed from the Shopping Cart.

The Remove button should change back to Add to Cart, and the cart badge should be updated accordingly.

## Actual Result

Clicking the Remove button produces no change. The product is not removed from the Shopping Cart.

## Severity

Medium

## Priority

Medium

## Status

New
