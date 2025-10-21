# 🧩 Software Testing Life Cycle (STLC)

STLC is a subset of SDLC that focuses on the testing phase of the software development process.  

---

| **Phase** | **Activities** | **Responsibilities** | **Outcome** | **Reference Documents** |
|------------|----------------|----------------------|--------------|---------------------------|
| **1️⃣ Requirement Analysis** | - Review SRD / BRD / FRD<br>- Interview stakeholders to gather more info<br>- Identify missing or incomplete requirements | - Business Analyst<br>- Stakeholders (Users)<br>- Test Manager<br>- Test Lead<br>- Test Engineers | - Clear & complete finalized requirements | - Project Plan (Project Timeline) |
| **2️⃣ Test Planning** | - Identify resources<br>- Team formation<br>- Test estimation<br>- Prepare test plan<br>- Review test plan<br>- Test plan sign-off | - Test Manager<br>- Test Lead<br>- Test Engineers | - Test Plan Document | - Project Plan (Timeline)<br>- Functional Requirement Document (FRD) |
| **3️⃣ Test Development** | - Prepare test scenarios (What to test)<br>- Prepare test cases (How to test)<br>- Review test cases<br>- Create Traceability Matrix (RTM)<br>- Test cases sign-off | - Test Lead<br>- Test Engineers | - Test Cases Document<br>- Traceability Matrix | - Project Plan (Timeline)<br>- FRD<br>- Test Plan<br>- Design Docs / UI Specs<br>- Use Cases / Wireframes |
| **4️⃣ Environment Setup & Test Execution** | - Environment setup (test bed)<br>- Execute test cases<br>- Prepare test report / log<br>- Identify defects<br>- Prepare defect report<br>- Report defects to developers | - Test Lead<br>- Test Engineers | - Status / Test Reports<br>- Defect Report | - FRD<br>- Test Plan<br>- Test Cases<br>- Build from Development Team |
| **5️⃣ Test Cycle Closure** | - Analyze test reports<br>- Analyze bug reporting<br>- Evaluate exit criteria | - Test Manager<br>- Test Lead<br>- Test Engineers | - Test Summary Reports | - Test Reports<br>- Defect Reports |

---

# 🧠 Key Testing Concepts

## 🟩 Use Case

**Definition:**  
A *Use Case* describes the **requirement** from the user's perspective.  
It contains three main elements:

- **Actor:** Who uses the application  
- **Action:** Specific steps or activities to achieve the goal  
- **Goal/Outcome:** Expected result of the user's interaction with the system  

---

### 📘 Example: *Buy a Product* 

**Use Case:** Buy a product  
- **Actor:** Customer  
- **Goal:** Purchase a specific product on the website  
- **Steps:**  
  - Browse the product catalog  
  - Select a product and add it to the cart  
  - Proceed to checkout  
  - Enter shipping and payment information  
  - Place the order  
  - Receive confirmation and tracking information  

---

## 🟦 Test Scenario

**Definition:**  
A *Test Scenario* represents a **possible area to be tested**.  
It identifies *what* to test, but not *how*.

### 📗 Example

**Test Scenario:** Successful purchase with a valid credit card  
- Covers a “happy path” where the customer completes the purchase successfully.

---

## 🟨 Test Case

**Definition:**  
A *Test Case* provides **step-by-step actions** to validate the functionality of the Application Under Test (AUT).  
It includes:
- **Test Steps**
- **Expected Result**
- **Actual Result**

---

### 📙 Example 

**Test Case ID:** TC01 – Purchase with valid credit card  
**Pre-conditions:** Customer has a valid account, and a product is added to the cart  
**Steps:**
1. Enter valid shipping address  
2. Enter valid credit card info (number, expiry, CVV)  
3. Click "Place Order"  
**Expected Result:**
- Order confirmation is displayed  
- Credit card is charged successfully  
- Order status reflects “Processing”

**Additional Test Cases:**
- **TC02:** Purchase with invalid credit card number  
- **TC03:** Purchase with insufficient funds  
- **TC04:** Purchase with missing shipping address  
- **TC05:** Purchase with guest checkout  

---

## 🟧 Requirement Traceability Matrix (RTM)

**Definition:**  
A *Requirement Traceability Matrix* is a **mapping between requirements and test cases**.  
Its main purpose is to ensure that **all requirements are covered by corresponding test cases.**

### 📋 Example 

| **Requirement ID** | **Requirement Description** | **Test Case ID’s** |
|--------------------|-----------------------------|--------------------|
| **REQ001** | User should be able to log in | TC001, TC002 |
| **REQ002** | System should display product details | TC003, TC004 |
| **REQ003** | User can add items to the shopping cart | TC005, TC006 |

---
