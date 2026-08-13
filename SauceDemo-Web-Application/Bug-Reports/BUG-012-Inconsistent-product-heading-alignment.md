# BUG-012 — Inconsistent Product Heading Alignment

## Summary

When logged in as `visual_user`, the product headings for Sauce Labs Bolt T-Shirt and Sauce Labs Fleece Jacket are right-aligned, while the other product headings are left-aligned.

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
3. Observe the alignment of the product headings.
4. Compare the headings for Sauce Labs Bolt T-Shirt and Sauce Labs Fleece Jacket with the other product headings.

## Expected Result

All product headings should have consistent alignment within their respective product cards.

## Actual Result

The headings for Sauce Labs Bolt T-Shirt and Sauce Labs Fleece Jacket are right-aligned, while the other product headings are left-aligned.

## Severity

Low

## Priority

Low

## Status

New
