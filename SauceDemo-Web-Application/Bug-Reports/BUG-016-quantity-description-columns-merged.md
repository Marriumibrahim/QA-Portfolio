# BUG-016 — Quantity and Description Columns Are Merged on Shopping Cart Page

## Summary

When logged in as `visual_user`, the Quantity and Description columns on the Shopping Cart page are incorrectly merged or displayed as a single column.

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
- At least one product has been added to the Shopping Cart.

## Steps to Reproduce

1. Log in using `visual_user`.
2. Add a product to the Shopping Cart.
3. Open the Shopping Cart.
4. Observe the table headings and product information.
5. Check the Quantity and Description columns.

## Expected Result

The Quantity and Description columns should be displayed as separate columns with proper alignment.

## Actual Result

The Quantity and Description columns are merged/misaligned and appear as a single column.

## Severity

Medium

## Priority

Medium

## Status

New
