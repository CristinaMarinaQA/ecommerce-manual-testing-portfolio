# Test Execution Report – E-commerce Web Application

---

## 1. Test Summary

Total Test Cases Executed: 15  
Passed: 12  
Failed: 3  
Blocked: 0  
Not Executed: 0  

---

## 2. Failed Test Cases

- TC-03: Registration with Invalid Email Format
- TC-09: Update Product Quantity in Cart
- TC-13: Registration with Extremely Long Input Data

---

## 3. Defects Summary

Total Defects Raised: 3  

| Bug ID  | Severity | Priority | Status |
|----------|----------|----------|--------|
| BUG-01   | High     | High     | New    |
| BUG-02   | High     | High     | New    |
| BUG-03   | Medium   | Medium   | New    |

---

## 4. Overall Test Result

Application core functionality works as expected.  
However, 2 critical issues were identified in the User Registration module and Cart Functionality, allowing account creation with an invalid email format, and the user was not able to update the quantity in the shopping cart. A medium severity issue was identified executing Boundary & Negative Testing, where the system did not restrict the length of the "Name" field.

---

## 5. Recommendations

- Implement proper email format validation and add an update quantity button in the shopping cart.
- Restrict the "Name" field length.
- Add server-side validation to prevent invalid data storage.
- Re-test the modules where the issues were found, after the fixes are deployed.
