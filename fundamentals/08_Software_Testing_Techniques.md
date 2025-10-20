# 🧪 Software Testing Techniques

---

## 1. Equivalence Class Partitioning (ECP)

- **Concept:**  
  Divide input data into equivalence classes (valid and invalid) to minimize the number of test cases while maintaining good coverage.  
  Each class represents a set of inputs that should behave similarly.
- **Example Table:**

| Equivalence Classes | Valid/Invalid | Test Data |
| --- | --- | --- |
| A..Z | Valid | XYZ |
| a..z | Valid | xyz |
| Special Characters | Invalid | @#$% |
| Spaces | Invalid | Xy z |
| Numbers | Invalid | 1234 |


---

## 2. Boundary Value Analysis (BVA)

- **Concept:**  
  Focus on testing boundaries or edge values of valid and invalid input ranges.  
  Errors are often found near the minimum or maximum boundaries.
- **Example Table:**

| Parameter | Data | Valid/Invalid |
| --- | --- | --- |
| Min | 18 | Valid |
| Min − 1 | 17 | Invalid |
| Min + 1 | 19 | Valid |
| Max − 1 | 34 | Valid |
| Max | 35 | Valid |
| Max + 1 | 36 | Invalid |


---

## 3. Decision Table-Based Testing (Cause-Effect Table)

- **Concept:**  
  Used when multiple conditions lead to different actions.  
  Helps ensure all combinations of inputs and corresponding outputs are covered.
- **Decision Table:**

| Conditions | Membership Type: Regular | Membership Type: Premium |
| --- | --- | --- |
| Purchase Amount < $50 | No Discount | 5% Discount |
| Purchase Amount ≥ $50 | 2% Discount | 10% Discount |

- **Expanded Test Cases:**

| Membership Type | Purchase Amount | Action/Outcome |
| --- | --- | --- |
| Regular | 0 (very low) | No Discount |
| Regular | < $50 | No Discount |
| Regular | = $50 (edge) | 2% Discount |
| Regular | > $50 | 2% Discount |
| Regular | 500 (large) | 2% Discount |
| Premium | 0 (very low) | 5% Discount |
| Premium | < $50 | 5% Discount |
| Premium | = $50 (edge) | 10% Discount |
| Premium | > $50 | 10% Discount |
| Premium | 500 (large) | 10% Discount |


---

## 4. State Transition Testing

- **Concept:**  
  The system’s behavior changes depending on its current state and user actions.  
  Testers verify valid and invalid transitions between states.
- **Example:** Login attempt system that locks the account after three failed tries.

**State Table:**

| State | Login | Correct Password → Next State | Incorrect Password → Next State |
| --- | --- | --- | --- |
| S1 | First attempt | S4 (Home Page) | S2 (Second attempt) |
| S2 | Second attempt | S4 (Home Page) | S3 (Third attempt) |
| S3 | Third attempt | S4 (Home Page) | S5 (Account locked) |
| S4 | Home Page | — | — |
| S5 | Account locked | — | Display: “Account locked. Please consult admin.” |


---

## 5. Error Guessing

- **Concept:**  
  Based on tester’s experience and intuition to predict where defects may occur.  
  It’s an exploratory technique, often used after applying formal methods like ECP or BVA.
- **Common Examples:**
  - Leaving a required field blank
  - Entering special characters in numeric fields
  - Typing more characters than allowed
  - Using invalid date formats
  - Skipping validation steps or using unexpected input order

---

## 🧩 Summary

| Category | Technique | Purpose |
| --- | --- | --- |
| Input Domain Testing | Equivalence Class Partitioning (ECP) | Divide inputs into valid/invalid ranges |
| Input Domain Testing | Boundary Value Analysis (BVA) | Test edge/boundary values |
| Logic-Based Testing | Decision Table Testing | Handle multiple condition–action combinations |
| State-Based Testing | State Transition Testing | Verify behavior across system states |
| Experience-Based | Error Guessing | Use tester’s intuition to find hidden defects |
