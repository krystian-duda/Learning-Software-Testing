# Test Plan: User Registration Functionality

**Project:** Automation Exercise
**Module:** User Management (Sign up)
**Author:** Krystian

## 1. Introduction
The goal of this test is to verify the robustness of the user registration form, ensuring it handles both valid and invalid data correctly.

## 2. Test Cases (Scenarios)
* **TC-01: Valid Registration** - Verify that a user can create an account using unique data.
* **TC-02: Empty Form Submission** - Verify system behavior when clicking "Signup" with empty fields.
* **TC-03: Invalid Email Format** - Verify validation when the email is missing '@' or domain.
* **TC-04: Boundary Testing & Character Validation (Username Field) – Verify how the system handles extremely long names and special characters. [STATUS: FAILED - See Bug Report #001]
* **TC-05: Duplicate Email** - Verify that the system prevents registering twice with the same email.

## 3. Test Environment
- **Browser:** Chrome
- **URL:** https://automationexercise.com/login
