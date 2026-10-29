# 🧪 Test Cases – Search & Delete Student Module

**Prepared By:** QA Tester  
**Date:** April 2025  

---

## Search Module – Total Test Cases: 8

| TC ID | Test Title | Test Data | Steps | Expected Result | Actual Result | Status |
|---|---|---|---|---|---|---|
| TC-SRC-001 | Valid naam se search hona chahiye | Search: Rahul | Search box mein "Rahul" type karo, Enter dabao | Rahul Sharma ka record dikhe | Record correctly display hua | ✅ Pass |
| TC-SRC-002 | Partial naam se search hona chahiye | Search: Rah | Search box mein "Rah" type karo | Rahul wale students dikhein | Partial search kaam kiya | ✅ Pass |
| TC-SRC-003 | Roll No se search hona chahiye | Roll No: 101 | Search mein 101 type karo | Roll No 101 wala student dikhe | Correct student display hua | ✅ Pass |
| TC-SRC-004 | Capital letters se search hona chahiye | Search: RAHUL | Search mein RAHUL type karo | Rahul ka record dikhe | Record mila | ✅ Pass |
| TC-SRC-005 | Non-existent student pe "No record found" aana chahiye | Search: XYZStudent999 | Search karo | "No records found" message dikhe | Correct message aaya | ✅ Pass |
| TC-SRC-006 | Special characters se page crash nahi hona chahiye | Search: @#$%^ | Search box mein @#$%^ type karo | "No records found" dikhe | Page error de raha tha | ❌ Fail |
| TC-SRC-007 | Search clear hone pe full list aani chahiye | — | Kuch search karo, phir search box clear karo | Saari students list dikhe | Full list wapas aayi | ✅ Pass |
| TC-SRC-008 | Search results mein data sahi hona chahiye | Search: Rahul | Search karo, details verify karo | Name, Roll No, Class sahi ho | Phone column mein email show ho raha tha | ❌ Fail |

---

## 📊 Search Summary

| Total | Pass | Fail |
|---|---|---|
| 8 | 6 | 2 |

---

## Delete Module – Total Test Cases: 6

| TC ID | Test Title | Steps | Expected Result | Actual Result | Status |
|---|---|---|---|---|---|
| TC-DEL-001 | Student successfully delete hona chahiye | Student ke aage Delete click karo, Confirmation mein OK dabao | Student delete ho aur list se hatay | Student successfully deleted | ✅ Pass |
| TC-DEL-002 | Delete ke baad list mein nahi dikhna chahiye | Student delete karo, list refresh karo | Deleted student list mein nahi ho | Student list se hat gaya | ✅ Pass |
| TC-DEL-003 | Cancel dabaane pe student delete nahi hona chahiye | Delete click karo, popup mein Cancel dabao | Student delete na ho | Student delete nahi hua | ✅ Pass |
| TC-DEL-004 | Delete se pehle confirmation popup aana chahiye | Delete button click karo | "Are you sure?" popup aaye | Confirmation popup aaya | ✅ Pass |
| TC-DEL-005 | Delete hue student ko search karne pe nahi milna chahiye | Student delete karo, phir search karo | "No records found" | Correct — no record found | ✅ Pass |
| TC-DEL-006 | Saare students delete hone pe "No students found" dikhe | Saare students delete karo | "No students found" message | Empty table, koi message nahi | ❌ Fail |

---

## 📊 Delete Summary

| Total | Pass | Fail |
|---|---|---|
| 6 | 5 | 1 |
