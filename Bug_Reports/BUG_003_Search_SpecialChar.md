# 🐛 BUG-003 – Search Mein Special Characters Se Page Error Aata Hai

| Field | Detail |
|---|---|
| **Bug ID** | BUG-003 |
| **Module** | Search Student |
| **Severity** | 🟡 Low |
| **Priority** | 🟠 Medium |
| **Status** | Open |
| **Found By** | QA Tester |
| **Date** | April 2025 |
| **Related TC** | TC-SRC-006 |

---

## Environment

| Field | Detail |
|---|---|
| OS | Windows 11 |
| Browser | Google Chrome |

---

## Steps to Reproduce

1. Admin login karo
2. Student list page pe jao
3. Search box mein type karo: `@#$%^`
4. Enter dabao

---

## Expected Result

```
"No records found" message aana chahiye
Application normal rehni chahiye
```

## Actual Result

```
Page ek error throw karta hai
Application crash jaisi ho jaati hai
User ko manually navigate karna padta hai
```

---

## Impact

- Application unstable lagti hai
- Poor user experience
- Security risk — SQL injection possible

---

## Suggested Fix

Search input pe special characters sanitize karo aur proper error handling add karo.

---

## Screenshot Evidence

> 📸 `Screenshots/BUG-003_SearchSpecialChar_Error.png`
