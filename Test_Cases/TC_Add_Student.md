# 🧪 Test Cases – Add Student Module

**Module:** Add Student  
**Prepared By:** QA Tester  
**Date:** April 2025  
**Total Test Cases:** 12  

---

| TC ID | Test Title | Test Data | Steps | Expected Result | Actual Result | Status |
|---|---|---|---|---|---|---|
| TC-ADD-001 | Valid data se student add hona chahiye | Name: Rahul Sharma, Roll: 101, Class: 10th, Age: 16, Email: rahul@test.com, Phone: 9876543210 | 1. Add Student click karo 2. Saare fields bharo 3. Submit karo | "Student added successfully" message aaye | Student successfully add hua | ✅ Pass |
| TC-ADD-002 | Student list mein dikhna chahiye add hone ke baad | Valid data | Student add karo, phir list open karo | Naya student list mein dikhe | Student list mein dikh raha tha | ✅ Pass |
| TC-ADD-003 | Submit ke baad form reset hona chahiye | Valid data | Student add karo | Form fields empty ho jaayein | Form reset ho gaya | ✅ Pass |
| TC-ADD-004 | Phone number 10 digits hona chahiye | Phone: 98765 (5 digits) | Invalid phone enter karo, submit karo | "Phone must be 10 digits" error | Validation error aaya | ✅ Pass |
| TC-ADD-005 | Duplicate Roll No allow nahi hona chahiye | Roll No: 101 (already exists) | Same Roll No se dobara student add karo | "Roll No already exists" error | Duplicate add ho gaya | ❌ Fail |
| TC-ADD-006 | Blank name pe error aana chahiye | Name: blank | Name blank rakhke submit karo | "Name is required" error | Form submit ho gaya blank name se | ❌ Fail |
| TC-ADD-007 | Blank Roll No pe error aana chahiye | Roll No: blank | Roll No blank rakhke submit karo | "Roll No is required" error | Validation error aaya | ✅ Pass |
| TC-ADD-008 | Invalid email accept nahi hona chahiye | Email: rahul@@test | Invalid email enter karo, submit karo | "Invalid email format" error | Invalid email accept ho gaya | ❌ Fail |
| TC-ADD-009 | Negative age accept nahi hona chahiye | Age: -5 | Negative age enter karo | "Age must be positive" error | Validation error aaya | ✅ Pass |
| TC-ADD-010 | Age 200 se zyada accept nahi hona chahiye | Age: 250 | Age 250 enter karo | "Invalid age" error | Error aaya | ✅ Pass |
| TC-ADD-011 | Name mein numbers accept nahi hone chahiye | Name: 12345 | Numbers as name enter karo | "Only alphabets allowed" error | Error aaya | ✅ Pass |
| TC-ADD-012 | Cancel button se form band hona chahiye | — | Cancel button click karo | Student list pe wapas aaye | Correctly redirect hua | ✅ Pass |

---

## 📊 Summary

| Total | Pass | Fail |
|---|---|---|
| 12 | 9 | 3 |
