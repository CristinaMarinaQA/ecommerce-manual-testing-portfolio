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

**Status:**
Pass

---

## Module: Cart Functionality

### TC-07: Add Product to Cart

**Precondition:** User is on Product Listing page  

**Steps:**
1. Navigate to Products page  
2. Click "Add to Cart" on any product  

**Expected Result:**  
Product is added to cart successfully and confirmation message is displayed.

**Actual Result:**  
Product was added successfully and confirmation message appeared.

**Status:**  
Pass

---

### TC-08: Remove Product from Cart

**Precondition:** Product is already added to cart  

**Steps:**
1. Navigate to Cart page  
2. Click "Remove" button for the product  

**Expected Result:**  
Product is removed from cart and cart is updated.

**Actual Result:**  
Product was removed successfully and cart updated.

**Status:**  
Pass

---

### TC-09: Update Product Quantity in Cart

**Precondition:** Product exists in cart  

**Steps:**
1. Navigate to Cart page  
2. Change product quantity  
3. Update cart  

**Expected Result:**  
Cart updates total price according to new quantity.

**Actual Result:**  
The update quantity button is not working and the quantity cannot be updated.

**Status:**  
Fail

---

## Module: Checkout Process

### TC-10: Successful Checkout with Valid Data

**Precondition:** Product exists in cart and user is logged in  

**Steps:**
1. Navigate to Cart  
2. Click "Proceed to Checkout"  
3. Confirm address details  
4. Place order  

**Expected Result:**  
Order is successfully placed and confirmation message is displayed.

**Actual Result:**  
Order was placed successfully and confirmation displayed.

**Status:**  
Pass

---

### TC-11: Checkout with Empty Mandatory Fields

**Precondition:** User is on checkout page  

**Steps:**
1. Leave mandatory fields empty  
2. Click "Place Order"  

**Expected Result:**  
System should display validation error messages.

**Actual Result:**  
System displayed validation messages for required fields.

**Status:**  
Pass

**Actual result:**
The system is displaying a message to fill out empty fields.

**Status:**
Pass

---

## Module: Boundary & Negative Testing

### TC-12: Registration with Minimum Password Length

**Precondition:** User is on Registration page  

**Steps:**
1. Enter valid name  
2. Enter valid unique email  
3. Enter password with minimum allowed length  
4. Click "Register"  

**Expected Result:**  
System accepts password if it meets minimum length requirement.

**Actual Result:**  
Password was accepted.

**Status:**  
Pass

---

### TC-13: Registration with Extremely Long Input Data

**Precondition:** User is on Registration page  

**Steps:**
1. Enter 256+ characters in Name field  
2. Enter valid email  
3. Enter valid password  
4. Click "Register"  

**Expected Result:**  
System should either limit input length or display validation message.

**Actual Result:**  
The account was created with extremy long name, 256+ characters in the name field.

**Status:**  
Fail

---

### TC-14: Add to Cart Without Being Logged In

**Precondition:** User is not logged in  

**Steps:**
1. Navigate to Products page  
2. Click "Add to Cart"  

**Expected Result:**  
System should allow guest cart functionality.

**Actual Result:**  
The product is added to the cart.

**Status:**  
Pass

---

### TC-15: Checkout with Empty Cart

**Precondition:** Cart is empty  

**Steps:**
1. Navigate to Cart  
2. Click "Proceed to Checkout"  

**Expected Result:**  
System should not display the checkout button when the cart is empty.

**Actual Result:**  
There is no button in the cart to checkout when it's empty.

**Status:**  
Pass
