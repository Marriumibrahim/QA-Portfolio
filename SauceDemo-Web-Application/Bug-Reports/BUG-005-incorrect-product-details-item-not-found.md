# BUG-005 — Fleece Jacket Opens Incorrect "ITEM NOT FOUND" Page

## Summary

When logged in as `problem_user`, clicking the Sauce Labs Fleece Jacket product from the Products page opens an incorrect Product Details page displaying an "ITEM NOT FOUND" message and unrelated content.

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
- Products page is displayed.

## Steps to Reproduce

1. Log in using `problem_user`.
2. Navigate to the Products page.
3. Locate **Sauce Labs Fleece Jacket**.
4. Click the **Sauce Labs Fleece Jacket** product name.
5. Observe the Product Details page.

## Expected Result

The Product Details page for **Sauce Labs Fleece Jacket** should be displayed with:

- Correct product name
- Correct product image
- Correct product description
- Correct product price
- Correct product actions

## Actual Result

An incorrect Product Details page is displayed containing:

- **"ITEM NOT FOUND"**
- Unrelated telephone-recording text
- `$√-1`
- A **Remove** button

The expected Sauce Labs Fleece Jacket product information is not displayed.

## Severity

High

## Priority

High

## Status

New
