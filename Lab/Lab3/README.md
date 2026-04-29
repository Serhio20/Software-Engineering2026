README.md
# UML Class Diagrams Repository


## 1. ATM System
**File:** `ATM.png`

**Description:**
This diagram provides a structural view of an ATM system. It clearly distinguishes between the logical entities (Customer, Transaction, BankSystem) and the hardware components associated with the `ATM_Terminal` class.

* **Key Classes:** `ATM_Terminal`, `BankSystem`, `Transaction`, `Card`.
* **Structural Highlights:** Uses composition to show that the ATM terminal is composed of hardware units like `CardReader`, `Screen`, `CashMachine`, and `Printer`.

## 2. Car Insurance System
**File:** `CarInsurance.png`

**Description:**
This model maps the data requirements for an insurance provider. It manages the lifecycle of a policy and the subsequent claims process.

* **Key Classes:** `Customer`, `InsurancePolicy`, `Claim`, `Document`, `InsuranceDatabase`.
* **Structural Highlights:** Illustrates the relationship between the `Claim` class and the `Document` class, emphasizing the document-centric nature of the claim submission process.

## 3. E-Shop System
**File:** `Eshop.png`

**Description:**
A domain model for an e-commerce application. This diagram focuses on the shopping cart logic, order fulfillment, and the role of the `Authenticator` service.

* **Key Classes:** `Customer`, `Product`, `ShoppingCart`, `Order`, `Authenticator`.
* **Structural Highlights:** Defines the relationship between the `Customer` and their `ShoppingCart`, and the transition from a `ShoppingCart` to an `Order`.

## 4. Medical Clinic System
**File:** `Medical.png`

**Description:**
This diagram represents the patient and record management system for a medical clinic, prioritizing data security and appointment scheduling.

* **Key Classes:** `Patient`, `Appointment`, `MedicalRecord`, `Authenticator`, `ClinicDatabase`.
* **Structural Highlights:** Emphasizes the dependency on the `Authenticator` class for secure data access and the strong relationship between `Patient` and their `MedicalRecord`.

---

