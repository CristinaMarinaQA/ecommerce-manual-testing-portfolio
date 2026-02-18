# Bug Reports – E-commerce Web Application

---

## BUG-01: System allows account creation with invalid email format

**Module:** User Registration  

**Severity:** High  

**Priority:** High  

**Environment:**
- OS: Windows 11
- Browser: Google Chrome (latest version)
- URL: https://automationexercise.com

---

### Preconditions:
User is on the Registration page.

---

### Steps to Reproduce:
1. Enter a valid name.
2. Enter an invalid email format (example: tiworkads38@gmailcom – missing dot before domain extension).
3. Enter a valid password.
4. Click "Register".

---

### Expected Result:
The system should validate email format and display an error message indicating an invalid email address format.  
Account should NOT be created.

---

### Actual Result:
The account was successfully created using an invalid email address format (tiworkads38@gmail.com).

