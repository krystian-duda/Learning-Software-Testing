# Bug Report #001: Missing character validation in Name field

**Status:** Open  
**Severity:** Low  
**Priority:** P3  

## Description
The "Name" field during registration accepts an excessively long string containing letters, numbers, and special characters: 'Test!@#$%^&*()_+1234567890Test!@#$%^&*()_+1234567890Test!@#$%^&*()_+1234567890Test!@#$%^&*()_+1234567890' 
without any validation.
The system fails to enforce character type restrictions and a maximum length limit.

## Environment
- **URL:** https://automationexercise.com/signup
- **Browser:** Chrome
- **Device:** Desktop

## Steps to Reproduce
1. Go to the Signup page.
2. In the "New User Signup!" section, enter a long string containing letters, numbers, and special characters: 'Test!@#$%^&*()_+1234567890Test!@#$%^&*()_+1234567890Test!@#$%^&*()_+1234567890Test!@#$%^&*()_+1234567890'
3. Enter a unique email and click "Signup".
4. Complete the registration process.

## Expected Result
The system should validate the Name field and only allow alphanumeric characters or display an error message for invalid symbols.

## Actual Result
The system accepts the long string with special characters and successfully creates the account without any length or character type validation.

## Evidence
1. **Initial Signup Stage:**
![Signup Input](username-signup-input.png)
<img width="1920" height="1080" alt="username-signup-input" src="https://github.com/user-attachments/assets/66a7be56-f603-437d-926e-d0ef071fcd13" />

2. **Detailed Registration Form (Validation Bypass):**
![Registration Form](username-detailed-form.png)
<img width="1920" height="1080" alt="username-detailed-form" src="https://github.com/user-attachments/assets/59c0725b-b5e4-4129-8167-c4fd8aebd7cd" />

3. **Final Account Confirmation:**
![Account Created](account-created-success.png)
<img width="1920" height="1080" alt="account-created-success" src="https://github.com/user-attachments/assets/7883c33e-6073-4cc9-9338-bd2904114601" />

4. **Impact - User Profile Display:**
![UI Bug](logged-in-username-ui-bug.png)
<img width="1920" height="1080" alt="logged-in-username-ui-bug" src="https://github.com/user-attachments/assets/46effb92-a9a0-46e8-b7ef-1f9d90415b4d" />

