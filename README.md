# SportHub — System Testing (SWT301)

System test documents for **SportHub**, a sports center management web app built in the SWP391 course. This repo holds the test cases and the defect list produced in SWT301 (Software Testing) at FPT University, 2026, by a 3-member team.

## About the system under test

- **Stack:** React + Vite (frontend), Spring Boot (backend), SQL Server
- **User roles:** Member, Receptionist, Coach, Manager
- **Requirements source:** SRS and 23 business rules (BR-01 to BR-23)

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

- Expected results are derived from the business rules, not from how the app currently behaves.
- Test design techniques: equivalence partitioning, boundary value analysis, state transition, decision table, experience-based testing.
- Each test case is linked to a business rule, and each defect is linked to a test case.

## Files

| File | Description |
|---|---|
| `SWT301_TestCase.xlsx` | Test cases per module, plus a test report |
| `DefectList.xlsx` | Defects exported from Jira (project SPH), with a summary dashboard |

## Defect tracking

Defects were logged in **Jira**. Each ticket has a summary, severity, environment, linked test case, steps to reproduce, expected result and actual result.

## Not covered

Email OTP, VNPay payment, the AI assistant, time-based rules, and QR/RFID/printer hardware were not tested because they depend on external services or devices.

## Note

SportHub was developed by a classmate's team in SWP391. This repo contains only the testing work.
