# SportHub — System Testing (SWT301)

My system test documents for **SportHub**, a sports center management web app built in the SWP391 course. This repo holds the test cases and the defect list I produced in SWT301 (Software Testing) at FPT University, 2026, as part of a 3-member team.

## About the system under test

- **Stack:** React + Vite (frontend), Spring Boot (backend), SQL Server
- **User roles:** Member, Receptionist, Coach, Manager
- **Requirements source:** SRS and business rules (BR-01 to BR-23)

## What was tested

Five modules, tested through the UI:

| Module | Scope |
|---|---|
| M1_PublicAuth | Guest pages, registration, login, role-based access |
| M2_MemberBooking | Packages, court booking, quota rules, vouchers, cancellation |
| M3_FrontDeskPOS | Check-in, POS payments, equipment loans |
| M4_CoachAI | Coach attendance, leave requests, workout plans |
| M5_AdminGovernance | Approvals, court maintenance, audit log |

## Approach

- Expected results are derived from the related business rules, not from how the app currently behaves.
- Test design techniques: equivalence partitioning, boundary value analysis, state transition, experience-based testing.
- Test cases are linked to business rules where one applies, and each defect is linked to the test case that found it.

## Results

- 60 test cases across 5 modules, executed 3 times with identical results: 52 passed, 8 failed.
- 8 defects logged in Jira (2 Major, 5 Minor, 1 Trivial), all still open at the time of testing.

## Files

| File | Description |
|---|---|
| `SWT301_TestCase_Nhat.xlsx` | Test cases per module, plus a test report |
| `DefectList_Nhat.xlsx` | Defects exported from Jira (project SPH), with a summary dashboard |

## Defect tracking

Defects were logged in **Jira**. Each ticket has a summary, severity, environment, linked test case, steps to reproduce, expected result and actual result.

## Not covered

Email OTP, VNPay payment, the AI assistant, time-based rules, and QR/RFID/printer hardware were not tested because they depend on external services or devices.

## Note

SportHub was developed by a classmate's team in SWP391. This repo contains only the testing work.
