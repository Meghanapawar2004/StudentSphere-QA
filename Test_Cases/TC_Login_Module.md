# 🧪 Test Cases – Login Module

**Module:** Login  
**Prepared By:** QA Tester  
**Date:** April 2025  
**Total Test Cases:** 10  

---

| TC ID | Test Title | Pre-condition | Test Data | Steps | Expected Result | Actual Result | Status |
|---|---|---|---|---|---|---|---|
| TC-LOG-001 | Valid login hona chahiye | App open hai | Email: admin@admin.com / Pass: admin | 1. URL open karo 2. Email bharo 3. Password bharo 4. Login click karo | Dashboard open ho | Dashboard open hua | ✅ Pass |
| TC-LOG-002 | Dashboard title correct hona chahiye | Login hua hai | Valid credentials | Login karo, page title check karo | "Dashboard" title dikhe | Title correct tha | ✅ Pass |
| TC-LOG-003 | Wrong password se login nahi hona chahiye | App open hai | Email: admin@admin.com / Pass: wrong123 | Wrong password enter karo, login click karo | Error message aaye | Error message aaya | ✅ Pass |
| TC-LOG-004 | Wrong email se login nahi hona chahiye | App open hai | Email: wrong@test.com / Pass: admin | Wrong email enter karo, login click karo | Error message aaye | Error message aaya | ✅ Pass |
| TC-LOG-005 | Blank email pe error aana chahiye | App open hai | Email: blank / Pass: admin | Email blank rakhke login karo | "Email is required" error | Koi error nahi aaya | ❌ Fail |
| TC-LOG-006 | Blank password pe error aana chahiye | App open hai | Email: admin@admin.com / Pass: blank | Password blank rakhke login karo | "Password is required" error | Koi error nahi aaya | ❌ Fail |
| TC-LOG-007 | Password masked dikhna chahiye | App open hai | Koi bhi password | Password field mein type karo | Dots/asterisk dikhein | Password masked tha | ✅ Pass |
| TC-LOG-008 | SQL Injection se login nahi hona chahiye | App open hai | Email: ' OR 1=1-- / Pass: anything | SQL inject karo, login try karo | Login fail ho | Login fail hua | ✅ Pass |
| TC-LOG-009 | Logout button kaam karna chahiye | Login hua hai | — | Logout button click karo | Login page pe aaye | Login page pe aaya | ✅ Pass |
| TC-LOG-010 | Logout ke baad back button se dashboard nahi kholna chahiye | Logout kiya hai | — | Browser back button dabao | Login page pe rahe | Login page pe raha | ✅ Pass |

---

## 📊 Summary

| Total | Pass | Fail |
|---|---|---|
| 10 | 8 | 2 |
