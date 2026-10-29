# 📋 Test Plan – Student Management System

**Project:** Student Management System – Manual Testing  
**Version:** 1.0  
**Prepared By:** QA Tester  
**Date:** April 2025  

---

## 1. Objective

Student Management System web application ka manual testing karna aur ensure karna ki sab features correctly kaam kar rahe hain.

---

## 2. Scope

### ✅ In Scope
- Login / Logout
- Add New Student
- View Student List
- Search Student
- Delete Student
- Form Validations

### ❌ Out of Scope
- Performance / Load Testing
- Mobile App Testing
- Payment Module

---

## 3. Test Environment

| Parameter | Detail |
|---|---|
| OS | Windows 11 |
| Browser | Google Chrome (Latest) |
| Application Type | Web Application |
| Internet | Required |

---

## 4. Test Approach

- **Positive Testing** – Valid data se test karna
- **Negative Testing** – Invalid/blank data se test karna
- **Boundary Testing** – Min/Max values test karna
- **UI Testing** – Buttons, labels, alignment check karna
- **Security Testing** – SQL injection, session check

---

## 5. Entry Criteria

- Application browser mein accessible hai
- Test cases ready hain
- Test data prepared hai

---

## 6. Exit Criteria

- Saare test cases execute ho gaye
- Saare Critical/High bugs report ho gaye
- Pass rate >= 70%
- Test summary report complete ho gayi

---

## 7. Deliverables

| Document | Location |
|---|---|
| Test Plan | `/docs/Test_Plan.md` |
| RTM | `/docs/RTM.md` |
| Test Cases | `/Test_Cases/` |
| Bug Reports | `/Bug_Reports/` |
| Test Summary | `/Test_Reports/` |
| Test Data | `/Test_Data/` |

---

## 8. Risk & Mitigation

| Risk | Mitigation |
|---|---|
| Site down ho jaye | Backup practice site use karein |
| Requirements unclear hon | Developer se clarify karein |
| Time kam ho | High priority TCs pehle execute karein |
