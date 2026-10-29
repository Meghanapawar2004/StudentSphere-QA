# 📊 RTM – Requirement Traceability Matrix

**Project:** Student Management System  
**Prepared By:** QA Tester  
**Date:** April 2025  

> RTM ensure karta hai ki koi bhi requirement untested na rahe.

---

## RTM Table

| Req ID | Requirement | Module | Test Case IDs | Status |
|---|---|---|---|---|
| REQ-001 | Admin valid credentials se login kar sake | Login | TC-LOG-001, TC-LOG-002 | ✅ Covered |
| REQ-002 | Invalid login block hona chahiye | Login | TC-LOG-003, TC-LOG-004 | ✅ Covered |
| REQ-003 | Blank fields pe error message aana chahiye | Login | TC-LOG-005, TC-LOG-006 | ✅ Covered |
| REQ-004 | Admin logout kar sake | Login | TC-LOG-009, TC-LOG-010 | ✅ Covered |
| REQ-005 | Naya student add ho sake | Add Student | TC-ADD-001, TC-ADD-002 | ✅ Covered |
| REQ-006 | Duplicate Roll No allow nahi hona chahiye | Add Student | TC-ADD-005 | ✅ Covered |
| REQ-007 | Required fields blank nahi ho sakte | Add Student | TC-ADD-006, TC-ADD-007 | ✅ Covered |
| REQ-008 | Valid email format required | Add Student | TC-ADD-008 | ✅ Covered |
| REQ-009 | Student naam se search ho sake | Search | TC-SRC-001, TC-SRC-002 | ✅ Covered |
| REQ-010 | Roll No se search ho sake | Search | TC-SRC-003 | ✅ Covered |
| REQ-011 | Invalid search pe "No record found" dikhe | Search | TC-SRC-005, TC-SRC-006 | ✅ Covered |
| REQ-012 | Student delete ho sake confirmation ke baad | Delete | TC-DEL-001, TC-DEL-002 | ✅ Covered |
| REQ-013 | Cancel karne pe student delete na ho | Delete | TC-DEL-003 | ✅ Covered |

---

## Coverage Summary

| Module | Total Requirements | Covered | Not Covered |
|---|---|---|---|
| Login | 4 | 4 | 0 |
| Add Student | 4 | 4 | 0 |
| Search | 3 | 3 | 0 |
| Delete | 2 | 2 | 0 |
| **Total** | **13** | **13** | **0** |

**Requirement Coverage: 100% ✅**
