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

### 3.2 Functional Testing
- Verifies that each feature or workflow behaves as intended.

### 3.3 Non-Functional Testing
- Evaluates performance, load, stress, reliability, and security.

### 3.4 Usability Testing
- Checks user-friendliness, clarity, and accessibility for end users.

---

 ## 4. User Acceptance Testing (UAT)
- Conducted by UAT or client team after system testing.

**Types**
- Alpha Testing: Conducted in company environment using internal data.
- Beta Testing: Conducted in client environment using real customer data.
