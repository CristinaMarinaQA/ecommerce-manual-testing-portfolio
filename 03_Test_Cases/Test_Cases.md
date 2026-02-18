# Test Cases – E-commerce Web Application

---

## Module: User Registration

### TC-01: Successful User Registration

**Precondition:** User is on Registration page  

**Steps:**
1. Navigate to Registration page  
2. Enter valid name  
3. Enter valid unique email  
4. Enter valid password  
5. Click "Register" button  

**Expected Result:**  
User account is created successfully and user is redirected to logged-in homepage.

**Actual Result:**  
User was redirected to homepage successfully and the acount is created.

**Status:**  
Pass

---

### TC-02: Registration with Existing Email

**Precondition:** User email already exists in system  

**Steps:**
1. Navigate to Registration page  
2. Enter valid name  
3. Enter existing email  
4. Enter valid password  
5. Click "Register"  

**Expected Result:**  
System displays error message: "Email already exists".

**Actual Result:**  
The system is displaying the error message: "Email already exists!".

**Status:**  
Pass


---

### TC-03: Registration with Invalid Email Format

**Precondition:** User is on Registration page  

**Steps:**
1. Enter name  
2. Enter invalid email format (example: useremail.com)  
3. Enter password  
4. Click "Register"  

**Expected Result:**  
System displays validation error for invalid email format.

**Actual Result:**  
The acoount was created with invalid email address format: tiworkads38@gmailcom.

**Status:**  
Fail

---

## Module: User Login

### TC-04: Login with Valid Credentials

**Precondition:** Registered user exists  

**Steps:**
1. Navigate to Login page  
2. Enter valid email  
3. Enter correct password  
4. Click "Login"  

**Expected Result:**  
User is logged in successfully and redirected to homepage.

**Actual Result:**
The user is logged in successfully and redirected to homepage.

**Status:**
Pass

---

### TC-05: Login with Incorrect Password

**Precondition:** Registered user exists  

**Steps:**
1. Enter valid email  
2. Enter incorrect password  
3. Click "Login"  

**Expected Result:**  
System displays error message: "Incorrect credentials".

**Actual result:**
The system is displaying error message: "Your email or password is incorrect!"

**Status:**
Pass

---

### TC-06: Login with Empty Fields

**Precondition:** User is on Login page  

**Steps:**
1. Leave email field empty  
2. Leave password field empty  
3. Click "Login"  

**Expected Result:**  
Validation message appears for required fields.

**Actual result:**
The system is displaying a message to fill out empty fields.

**Status:**
Pass
