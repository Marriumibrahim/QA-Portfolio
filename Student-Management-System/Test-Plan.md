# Test Plan
## Document Information

| Item | Details |
|------|---------|
| Project | Student Management System |
| Document | Test Plan |
| Version | 1.0 |
| Prepared By | Marrium Ibrahim |
| Date | August 2026 |
| Document Status | Draft |

## Project Overview

The Student Management System (SMS) is a web-based application designed to help students manage their academic activities. The application enables students to securely log in, register, view attendance records, access homework, check grades, receive notifications, update profile information, change passwords, and log out securely.

This test plan defines the testing strategy, scope, objectives, and deliverables required to verify that the application meets the specified functional requirements and quality standards.

## Test Objective
The primary objectives of testing are to:

- Verify that all functional requirements are implemented correctly.
- Ensure the application behaves as expected under normal user conditions.
- Identify defects before release.
- Validate business rules and data accuracy.
- Verify that fixed defects are successfully retested.
- Ensure the application provides a reliable and user-friendly experience.
- Ensure defects are documented with sufficient information for developers to reproduce and resolve them.

## Scope of Testing

This test plan covers the functional testing activities for the Student Management System. The scope includes verification of all core student-facing features and validation of the application's business requirements.
The following modules are included in the scope:

- User Login
- Student Registration
- Dashboard
- Attendance
- Homework
- Grades
- Notifications
- Student Profile
- Change Password
- Logout

The testing activities include:

- Functional Testing
- Regression Testing
- Smoke Testing
- Sanity Testing
- Exploratory Testing
- Bug Verification
- Retesting of Fixed Defects

 ## Out of Scope

The following testing activities are outside the scope of this test plan:

- Performance Testing
- Load Testing
- Stress Testing
- Security Testing
- Compatibility Testing across multiple browsers and devices
- User Acceptance Testing (UAT)

 ## Test Environment

## Test Environment

| Item | Details |
|------|---------|
| Application Type | Web Application |
| Operating System | Windows 11 |
| Browser | Google Chrome (Latest Stable Version) |
| Database | SQL Server |
| Testing Type | Manual Testing |
| Test Data | Sample Student Accounts |

## Entry Criteria

Testing will begin when:

- Business requirements have been reviewed and approved.
- Test environment is available.
- Test data has been prepared.
- A stable application build has been deployed to the test environment.
- Test cases have been reviewed and approved.

 ## Exit Criteria

Testing will be considered complete when:

- All planned test cases have been executed.
- All Critical and High severity defects have been resolved or deferred with approval.
- Regression testing has been completed successfully.
- Smoke testing has passed.
- Test Summary Report has been prepared.

## Test Deliverables

The following deliverables will be produced during the testing phase:

- Test Plan
- Test Scenarios
- Test Cases
- Bug Reports
- Regression Test Checklist
- Exploratory Testing Notes
- Test Summary Report

## Risks and Assumptions

### Risks

- Delay in application build delivery.
- Incomplete or changing requirements.
- Limited availability of test data.
- Environment-related issues.

### Assumptions

- The test environment is stable.
- Required test accounts are available.
- Business requirements are approved before testing begins.

## Approval

| Role | Name | Status |
|------|------|--------|
| QA Engineer | Marrium Ibrahim | Approved |

## Test Approach

Testing will be performed manually using black-box testing techniques. The application will undergo smoke testing after each new build, followed by functional testing, exploratory testing, and regression testing before release. Defects will be reported, verified after fixes, and retested to ensure successful resolution.
