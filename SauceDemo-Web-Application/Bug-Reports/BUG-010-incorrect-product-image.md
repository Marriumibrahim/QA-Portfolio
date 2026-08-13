# BUG-010 — Incorrect Product Image Displayed for Sauce Labs Backpack

## Summary

When logged in as `visual_user`, the Sauce Labs Backpack product displays an incorrect product image on the Products page.

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
3. Locate the Sauce Labs Backpack product.
4. Observe the product image displayed for Sauce Labs Backpack.

## Expected Result

The Sauce Labs Backpack should display its correct product image with appropriate dimensions and proportions.

## Actual Result

The Sauce Labs Backpack displays an incorrect product image.

The image also appears visually different in size compared with the expected product image.

## Severity

Medium

## Priority

Medium

## Status

New
