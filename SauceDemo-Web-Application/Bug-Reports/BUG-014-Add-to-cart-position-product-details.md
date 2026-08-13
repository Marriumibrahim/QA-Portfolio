# BUG-014 — Add to Cart Button Incorrectly Positioned on Product Details Page

## Summary

When logged in as `visual_user`, the Add to Cart button is incorrectly positioned on the Product Details page.

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
- Products page is displayed.

## Steps to Reproduce

1. Log in using `visual_user`.
2. Navigate to the Products page.
3. Select any product.
4. Observe the Product Details page.
5. Observe the position of the Add to Cart button.

## Expected Result

The Add to Cart button should be correctly positioned and aligned within the Product Details page layout.

## Actual Result

The Add to Cart button is incorrectly positioned on the Product Details page.

## Severity

Medium

## Priority

Medium

## Status

New
