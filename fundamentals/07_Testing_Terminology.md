# 🧪 Testing Terminology

## 🔁 Regression Testing
Regression testing is the process of testing a software application to ensure that **new changes** (such as updates, bug fixes, or new features) do **not negatively impact existing functionality**.

### Types of Regression Testing
- **Unit Regression Testing**
  - Test only the **specific changes** made by the developer.
- **Regional Regression Testing**
  - Test the **modified part** along with **connected modules**.
  - An **Impact Analysis Meeting** is conducted between testers and developers to identify affected areas.
- **Full Regression Testing**
  - Test the **main changed parts** and **the rest of the software** to ensure overall stability.
  - Usually performed when **many changes** have been made.

---

## 🔁 Re-Testing
- Performed **after a bug fix** to verify that the defect has been successfully resolved.  
- **Focuses on the same test cases** that previously failed.

### Re-Testing vs Regression Testing
| Aspect | Re-Testing | Regression Testing |
|--------|-------------|--------------------|
| Purpose | To verify that a specific bug fix works | To ensure new changes don’t break existing features |
| Trigger | Developer fixes a bug | Any kind of change (bug fix, new feature, update) |
| Scope | Limited to the fixed defect | Covers related areas of the application |
| Relation | Subset of regression testing | Superset including re-testing |

---

## 🚀 Smoke Testing (Build Verification Test - BVT)
A **quick and basic test** to check whether the software is **stable enough** for deeper testing.

- Installation / Initial build verification  
- Basic screens and core features appear correctly  

---

## 🔥 Sanity Testing
A **basic functional check** after smoke testing, performed when the build is already stable.  
Used to verify **specific functionalities** before proceeding with detailed testing.

- Example:
  - Sign up  
  - Login  
  - Navigation  

> 🟡 Both **Smoke Testing** and **Sanity Testing** are entry-level tests.  
> Any bugs found here are considered **high severity and high priority**.

---

## 🕵️ Exploratory Testing
- Tester **has no prior knowledge** of the application.  
- The goal is to **learn and explore** functionalities through actual usage.  
- Common when **no documentation** (like test cases or requirements) exists.  

**Drawbacks**
- May **misinterpret features as bugs**  
- **Time-consuming** (self-learning required)

---

## 🎯 Adhoc Testing
- Conducted **without formal test cases or documentation**  
- Tester **has partial knowledge** of the system  
- Aim: **intentionally try to break** the application  
- Informal, **unplanned** activity

---

## 🐒 Monkey Testing
- Conducted **without any test cases or requirements**  
- Tester **has no knowledge** of the application  
- Aim: **break the system** randomly  
- Commonly used for **gaming or UI stress testing**

### Comparison: Exploratory vs Adhoc vs Monkey Testing

| Type | Tester Knowledge | Documentation | Goal |
|------|------------------|----------------|------|
| Exploratory | None | None | Learn & discover functionality |
| Adhoc | Some | None | Randomly break the system |
| Monkey | None | None | Randomly break the system |

---

## ➕ Positive Testing
- Testing with **valid data** → results in **expected success**.

## ➖ Negative Testing
- Testing with **invalid data** → results in **expected failure**.

---

## 🔄 End-to-End Testing
- Testing the **entire application flow** from **start to finish**.  
- Ensures that **all integrated components** work together correctly.

---

## 🌍 Globalization Testing
- Ensures the software functions **across different regions and cultures**.  
- Verifies:
  - Multiple **languages**
  - **Date/time formats**
  - **Currencies**
- Goal: Software can **work globally** without issues.

---

## 📍 Localization Testing
- Ensures the software is **adapted for a specific locale or audience**.  
- Verifies:
  - **Language translations**
  - **Cultural preferences**
  - **Regional settings**
- Goal: Software fits **specific cultural and linguistic needs**.

---
