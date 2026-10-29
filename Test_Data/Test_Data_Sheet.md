# 📋 Test Data Sheet – Student Management System

**Prepared By:** QA Tester  
**Date:** April 2025  

---

## 1. Valid Login Data

| # | Username | Password | Expected |
|---|---|---|---|
| 1 | admin@admin.com | admin | ✅ Login Success |
| 2 | admin@admin.com | Admin@123 | ✅ Login Success |

---

## 2. Invalid Login Data

| # | Username | Password | Expected |
|---|---|---|---|
| 1 | wrong@test.com | admin | ❌ Login Fail |
| 2 | admin@admin.com | wrongpass | ❌ Login Fail |
| 3 | (blank) | admin | ❌ Validation Error |
| 4 | admin@admin.com | (blank) | ❌ Validation Error |
| 5 | ' OR 1=1-- | anything | ❌ Login Fail (Security) |

---

## 3. Valid Student Data

| # | Name | Roll No | Class | Age | Email | Phone |
|---|---|---|---|---|---|---|
| 1 | Rahul Sharma | 101 | 10th | 16 | rahul@test.com | 9876543210 |
| 2 | Priya Singh | 102 | 9th | 15 | priya@test.com | 9876543211 |
| 3 | Amit Kumar | 103 | 11th | 17 | amit@test.com | 9876543212 |
| 4 | Neha Gupta | 104 | 10th | 16 | neha@test.com | 9876543213 |

---

## 4. Invalid Student Data

| # | Field | Invalid Value | Expected Error |
|---|---|---|---|
| 1 | Name | (blank) | "Name is required" |
| 2 | Roll No | (blank) | "Roll No is required" |
| 3 | Roll No | 101 (duplicate) | "Roll No already exists" |
| 4 | Email | rahul@@test | "Invalid email format" |
| 5 | Email | rahultest.com | "Invalid email format" |
| 6 | Phone | 98765 | "Must be 10 digits" |
| 7 | Phone | abcdefghij | "Only numbers allowed" |
| 8 | Age | -5 | "Must be positive number" |
| 9 | Age | 250 | "Invalid age" |
| 10 | Name | 12345 | "Only alphabets allowed" |

---

## 5. Search Test Data

| # | Search Input | Expected Result |
|---|---|---|
| 1 | Rahul | Rahul Sharma dikhna chahiye |
| 2 | Rah | Partial match — Rahul dikhna chahiye |
| 3 | 101 | Roll No 101 wala student |
| 4 | RAHUL | Case insensitive — Rahul milna chahiye |
| 5 | XYZStudent999 | "No records found" |
| 6 | @#$%^ | "No records found" (currently BUG-003) |
| 7 | (blank) | Saari students list |

---

## 6. Boundary Value Data

| Field | Min Valid | Max Valid | Below Min | Above Max |
|---|---|---|---|---|
| Age | 1 | 100 | 0 — invalid | 101 — invalid |
| Phone | 10 digits | 10 digits | 9 digits — invalid | 11 digits — invalid |
| Roll No | 1 | 9999 | 0 — invalid | 10000 — invalid |
| Name Length | 2 chars | 50 chars | 1 char — invalid | 51 chars — invalid |
