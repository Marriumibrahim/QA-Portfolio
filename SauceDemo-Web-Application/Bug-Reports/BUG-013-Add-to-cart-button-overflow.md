# BUG-013 — Add to Cart Button Overflows Product Card

## Summary

When logged in as `visual_user`, the Add to Cart button for Test.allTheThings() T-Shirt (Red) extends outside the product card/container.

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
3. Locate Test.allTheThings() T-Shirt (Red).
4. Observe the position of the Add to Cart button.

## Expected Result

The Add to Cart button should remain completely inside the product card/container and maintain proper alignment with the other product buttons.

## Actual Result

The Add to Cart button for Test.allTheThings() T-Shirt (Red) extends outside the product card/container.

## Severity

Medium

## Priority

Medium

## Status

New
