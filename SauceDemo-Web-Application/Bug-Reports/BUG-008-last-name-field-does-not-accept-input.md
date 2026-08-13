# BUG-008 — Last Name Field Does Not Accept Input

## Summary

When logged in as `error_user`, the Last Name field on the Checkout: Your Information page does not accept user input.

## Environment

| Item | Details |
|------|---------|
| Application | SauceDemo Web Application |
| User | error_user |
| Browser | Google Chrome |
| Operating System | Windows 11 |
| Test Type | Functional / Exploratory Testing |

## Preconditions

- SauceDemo application is accessible.
- User is logged in as `error_user`.
- At least one product has been added to the Shopping Cart.

## Steps to Reproduce

1. Log in using `error_user`.
2. Add a product to the Shopping Cart.
3. Open the Shopping Cart.
4. Click the **Checkout** button.
5. Enter a valid First Name.
6. Click the **Last Name** field.
7. Attempt to enter a valid Last Name.
8. Observe the Last Name field.

## Expected Result

The Last Name field should accept and retain the entered value.

The entered Last Name should be displayed correctly in the Last Name field.

## Actual Result

The Last Name field does not accept user input.

The user is unable to enter a Last Name.

## Severity

High

## Priority

High

## Status

New
