# 🔹 Testing Levels in the V-Model

## 1. Unit Testing
- Conducted on a single module or component.
- White-box testing performed by developers.

**Techniques**
- Basis Path Testing: All lines of code execute at least once.
- Control Structure Testing:
  - Conditional Coverage: Use both valid and invalid inputs.
  - Loop Coverage (Mutation Testing): Verify iteration behavior.

---

## 2. Integration Testing
- Performed between two or more modules.
- Checks data communication between modules.

**Types**
- Incremental:
  - Top-Down: Add child modules; use stubs for unfinished ones.
  - Bottom-Up: Add parent modules; use drivers for unfinished ones.
- Non-Incremental: Integrate all modules at once.

---

## 3. System Testing
- Verifies the entire system’s functionality.
- Black-box testing conducted by QA team after integration.
- Requires a clear understanding of client requirements.

### 3.1 User Interface Testing
- Ensures all UI elements are displayed correctly and responsive.
- Tests the UI of the application, focusing on:
  - UI element check, alignment check, error message readability.
  - Resolution, font, image, spelling, and overall attractiveness.
  - Scrollbar and hyperlink color consistency.
- **GUI Testing Checklist** should be prepared.
- Must refer to the **UI Specification Document (UI Spec)**.
  - The UI Spec contains **wireframes (dummy screens)** used for reference.

### 3.2 Functional Testing
- Verifies that each feature or workflow behaves as intended.

**Sub-Tests**
- **Object Properties Testing:**  
  Check properties such as placeholder text, enabled/disabled state, target="_blank", visibility, and focus.
- **Database Testing:**  
  Validate backend operations (DML – Data Manipulation Language): `INSERT`, `UPDATE`, `DELETE`, `SELECT`.
- **Error Handling Testing:**  
  Error messages must be simple, clear, and easily understandable.
- **Calculations/Manipulations Testing:**  
  Verify mathematical logic, e.g., interest, bonus, withdrawal amounts.
- **Links Testing:**
  - *Internal links:* navigation within the same page.
  - *External links:* navigation to a different page within the same application.
  - *Broken links:* invalid or missing targets (e.g., “Page Not Found”).
- **Cookies & Sessions Testing:**
  - *Cookies:* Temporary browser-side files created during browsing; auto-fill login or form data.
  - *Sessions:* Server-side time slots that expire after inactivity (e.g., auto-logout after several minutes).
  - Relation: **Cookies = Browser side, Sessions = Server side.**
### 3.3 Non-Functional Testing
- Evaluates performance, load, stress, reliability, and security.

### 3.4 Usability Testing
- Checks user-friendliness, clarity, and accessibility for end users.
- Evaluates overall **easiness of the application** setup and use.
- Ensures **help documents or user manuals** are readable and context-sensitive (e.g., tooltip help).

---

 ## 4. User Acceptance Testing (UAT)
- Conducted by UAT or client team after system testing.

**Types**
- Alpha Testing: Conducted in company environment using internal data.
- Beta Testing: Conducted in client environment using real customer data.
