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

#### 🔸 Sub-Tests
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
- **Only performed after Functional Testing is completed.**

#### 🔸 1. Performance Testing
- Tests **speed, responsiveness, and stability** of the application.

**Types**
- **Load Testing:**  
  - Checks performance (response time, turnaround time, throughput) with *expected load*.  
  - **Goal:** Ensure the application can handle expected load.
- **Stress Testing:**  
  - Gradually increase load beyond expected levels.  
  - **Goal:** Identify the breaking point of the application.
- **Endurance (Soak) Testing:**  
  - Evaluates long-term stability (e.g., 1+ month) under expected load.  
  - **Focus:** Time and stability of the application.  
  - **Goal:** Assess long-term reliability.
- **Spike Testing:**  
  - Suddenly increase load beyond expected limit.  
  - **Goal:** Evaluate how the system handles sudden traffic bursts.
- **Volume Testing:**  
  - Tests how the application handles large volumes of data.  
  - **Goal:** Verify data processing capacity.

> 🔹 **Relation:**  
> - Load ↔ Endurance = sustained load stability  
> - Stress ↔ Spike = overload tolerance


#### 🔸 2. Security Testing
- Ensures the software is secure and protects sensitive information.

**Focus Areas**
- **Authentication:** Valid user verification.  
- **Authorization:** Permission validation for authenticated users.  
- **Network Security:** Detect vulnerabilities (virus, malware, etc.).  
- **Data Encryption & Decryption:** Protect data in transmission and storage.


#### 🔸 3. Recovery Testing
- Checks whether data is automatically saved or restored after unexpected events (e.g., crash, power failure).


#### 🔸 4. Compatibility Testing
- Verifies whether the application works correctly across different environments.

**Types**
- **OS Compatibility:** Different operating systems.  
- **Browser Compatibility (Cross-Browser Testing):** Multiple browsers.  
- **Hardware Compatibility (Configuration Testing):** Different device configurations.  
- **Forward Compatibility:** Future versions of OS/browser/hardware.  
- **Backward Compatibility:** Previous versions of OS/browser/hardware.


#### 🔸 5. Configuration Testing
- Ensures the application works correctly with various system configurations (e.g., RAM size, CPU, network setup).


#### 🔸 6. Installation Testing
- Verifies successful installation and uninstallation.  
- Checks whether installation steps are clear, screens are simple, and updates are handled automatically based on user choice.


#### 🔸 7. Sanitation (Garbage) Testing
- Detects unnecessary or extra features beyond requirements.  
- If the application provides unrequested features, they are considered **bugs**.

---

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
