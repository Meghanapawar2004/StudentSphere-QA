# 🐛 BUG-002 – Duplicate Roll No se Student Add Ho Jaata Hai

| Field | Detail |
|---|---|
| **Bug ID** | BUG-002 |
| **Module** | Add Student |
| **Severity** | 🟠 Medium |
| **Priority** | 🔴 High |
| **Status** | In Progress |
| **Found By** | QA Tester |
| **Date** | April 2025 |
| **Related TC** | TC-ADD-005 |

---

## Environment

| Field | Detail |
|---|---|
| OS | Windows 11 |
| Browser | Google Chrome |

---

## Steps to Reproduce

1. Admin login karo
2. Add Student → Roll No **101**, Name: Rahul Sharma → Submit
3. Student successfully add hoga
4. Dobara Add Student → Same Roll No **101**, Name: Priya Singh → Submit

---

## Expected Result

```
"Roll No 101 already exists. Please use a different Roll No."
error message aana chahiye
```

## Actual Result

```
Dono students same Roll No 101 ke saath add ho jaate hain
Koi error nahi aata
Student list mein duplicate entries dikhti hain
```

---

## Impact

- System mein duplicate data
- Roll No unique identifier hota hai — data integrity khatam
- Reports aur results galat ho sakte hain

---

## Suggested Fix

Database mein Roll No field ko UNIQUE set karo aur backend mein insert se pehle duplicate check lagao.

---

## Screenshot Evidence

> 📸 `Screenshots/BUG-002_DuplicateRollNo.png`
