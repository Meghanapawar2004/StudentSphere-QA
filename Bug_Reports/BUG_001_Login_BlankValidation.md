# 🐛 BUG-001 – Login Form Blank Fields Validation Missing

| Field | Detail |
|---|---|
| **Bug ID** | BUG-001 |
| **Module** | Login |
| **Severity** | 🔴 High |
| **Priority** | 🔴 High |
| **Status** | Open |
| **Found By** | QA Tester |
| **Date** | April 2025 |
| **Related TC** | TC-LOG-005, TC-LOG-006 |

---

## Environment

| Field | Detail |
|---|---|
| OS | Windows 11 |
| Browser | Google Chrome |
| App | Student Management System |

---

## Steps to Reproduce

1. Application URL browser mein open karo
2. Email field **bilkul blank** chod do
3. Password mein `admin` type karo
4. Login button click karo

---

## Expected Result

```
"Email is required" ya "Please fill all fields"
error message dikhna chahiye
```

## Actual Result

```
Page sirf refresh ho jaata hai
Koi error message nahi aata
User confuse ho jaata hai
```

---

## Impact

- User ko pata nahi chalta kya galat hua
- Bad user experience
- Basic validation missing hai

---

## Suggested Fix

Email aur Password fields pe required validation add karo — blank hone pe red border aur error message show ho.

---

## Screenshot Evidence

> 📸 `Screenshots/BUG-001_BlankLogin_NoError.png`
