# BUG-004 — Shopping Cart Badge Count Not Updated After Removing Products

## Summary

When logged in as `problem_user`, the Shopping Cart badge does not correctly update after products are removed from the cart.

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
- Products are available on the Products page.

## Steps to Reproduce

1. Log in using `problem_user`.
2. Add multiple products to the Shopping Cart.
3. Open the Shopping Cart.
4. Remove all products from the cart.
5. Observe the cart badge count.
6. Add another product to the cart.
7. Observe the cart badge count again.
8. Open the Shopping Cart and compare the badge count with the actual number of products.

## Expected Result

- The cart badge should accurately reflect the number of products currently in the Shopping Cart.
- After removing all products, the cart badge should display 0 or disappear.
- After adding one product to an empty cart, the cart badge should display 1.

## Actual Result

- After removing all products, the cart badge continued to display 1 even though the cart was empty.
- After adding another product, the cart badge displayed 2 even though only one product was present in the cart.

## Severity

Medium

## Priority

Medium

## Status

New
