# BUG-009 — Checkout Continues Without Required Last Name

## Summary

When logged in as `error_user`, the checkout process allows the user to proceed to the Checkout: Overview page even though the required Last Name field is empty.

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
6. Leave the **Last Name** field empty.
7. Enter a valid Postal Code.
8. Click the **Continue** button.
9. Observe the resulting page.

## Expected Result

An error message such as **"Last Name is required"** should be displayed.

The user should remain on the **Checkout: Your Information** page until all required fields are completed.

## Actual Result

No Last Name validation error is displayed.

The user is redirected to the **Checkout: Overview** page even though the required Last Name field is empty.

## Severity

High

## Priority

High

## Status

New
