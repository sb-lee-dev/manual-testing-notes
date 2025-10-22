# 🐞 Bug Reporting in Test Execution

---

## 💡 Defects

- **Definition:** Any mismatched functionality found in the application.  
- When reporting a defect, we must assign both **Severity** and **Priority**.

---

## ⚖️ Severity

- Indicates **how much impact** a defect has on the application.  
- **Decided by:** Tester  
- **Only testers** can change it.

| **Severity Level** | **Description** | **Examples** |
|---------------------|-----------------|---------------|
| **Blocker (Show Stopper)** | Testing or usage cannot proceed further. | - Smoke/Sanity testing fails<br>- Application crash<br>- Login not working |
| **Critical** | Main or core functionality not working. | - Fund transfer fails in net banking<br>- Product ordering fails in e-commerce |
| **Major** | Some undesirable behavior but still functional. | - No confirmation message after sending an email<br>- No confirmation after food order |
| **Minor** | No major breakdown; only cosmetic issues. | - Look and feel issue<br>- Spelling or alignment issue |

---

## 🚦 Priority

- Defines **how soon** the issue needs to be resolved.  
- **Can be changed** by other team members (not only testers).

| **Priority Level** | **Meaning** |
|---------------------|-------------|
| **P1 – High** | Must be resolved immediately. |
| **P2 – Medium** | Can wait until a new version or build is created. |
| **P3 – Low** | Can be fixed in later releases. |

---

## 📋 Combined Examples: Priority vs Severity  
*(Including common e-commerce defects)*

| **Issue / Bug Description** | **Priority** | **Severity** |
|------------------------------|--------------|---------------|
| A spelling mistake in a page not frequently navigated by users. | Low | Low |
| Application crashing in some very corner case. | Low | High |
| Slight change in logo colour or spelling mistake in company name. | High | Low |
| Issue with login functionality (user not able to login). | High | High |
| Web page not found when user clicks on a rarely visited link. | Low | High |
| Any cosmetic or spelling issues within a paragraph or page. | Low | Low |
| Unable to Add Items to Cart | High | Critical |
| Incorrect Price Calculation at Checkout | High | High |
| Broken Search Functionality | Medium | High |
| Missing Product Images | Low | Moderate |
| Inconsistent Product Availability Information | High | High |
| Slow Loading Times on Product Pages | Medium | Moderate |
| Non-Responsive Design on Mobile Devices | High | High |
| Incorrect Order Confirmation Emails | Medium | High |
| Payment Gateway Integration Failure | High | Critical |
| Unreliable Inventory Tracking | High | High |

---

## 🔁 Defect (Bug) Life Cycle
<img width="90%" height="auto" alt="defectLifeCycle" src="https://github.com/user-attachments/assets/bafc8b1d-a52c-451d-9fff-722827d965ff" />

---

## 🧩 Defect Resolution

**Definition:** Developer’s decision or disposition for a reported defect.

| Resolution Type | Description |
|---|---|
| Accept | Defect is valid and will be addressed. |
| Reject | Defect is not valid (works as intended / invalid report). |
| Duplicate | Same issue already exists in the tracker. |
| Enhancement | Request is an improvement, not a defect. |
| Need more information | Additional details/steps/logs are required. |
| Not reproducible | Issue cannot be reproduced with the given steps. |
| Fixed | Code change applied; awaiting verification. |
| As designed | Behavior matches current design/specification. |
