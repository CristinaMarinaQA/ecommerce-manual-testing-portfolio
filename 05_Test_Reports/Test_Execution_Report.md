# Test Execution Report – E-commerce Web Application

---

## 1. Test Summary

Total Test Cases Executed: 11  
Passed: 9  
Failed: 2  
Blocked: 0  
Not Executed: 0  

---

## 2. Failed Test Cases

- TC-03: Registration with Invalid Email Format
- TC-09: Update Product Quantity in Cart

---

## 3. Defects Summary

Total Defects Raised: 2  

| Bug ID  | Severity | Priority | Status |
|----------|----------|----------|--------|
| BUG-01   | High     | High     | New    |
| BUG-02   | High     | High     | New    |
---

## 4. Overall Test Result

Application core functionality works as expected.  
However, a critical validation issue was identified in the User Registration module, allowing account creation with invalid email format. Also a critical issue is that the user is not able to update the quantity in the shopping cart.

---

## 5. Recommendations

- Implement proper email format validation and add an update quantity button in the shopping cart.
- Add server-side validation to prevent invalid data storage.
- Re-test the registration module and update the quantity in the shopping cart after the fix deployed.
