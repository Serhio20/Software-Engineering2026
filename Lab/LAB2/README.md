README.md
# UML Use Case Diagrams Repository


---

## 1. ATM System
**File:** `atm.png`

**Description:**
This diagram models the interaction between a Customer and an automated banking system. It outlines the core functionalities required for a typical ATM transaction session.

* **Actors:** Customer, Bank System.
* **Key Use Cases:**
    * `Authenticate`: Mandatory prerequisite for banking operations (`<<include>>`).
    * `Check Balance`: Extends to `Display Balance` when a user chooses to view the amount.
    * `Withdraw Cash`: Extends to `Print Receipt` based on user preference.

## 2. Car Insurance System
**File:** `car insurance.png`

**Description:**
This diagram represents the registration and claim processing workflow for an insurance provider. It distinguishes between the capabilities of new users and existing registered users.

* **Actors:** New Customer, Registered Customer, Insurance Database.
* **Key Use Cases:**
    * `Authenticate`: Required for secure policy purchase and claim submission.
    * `Calculate Quote`: Publicly accessible use case for new customers.
    * `Purchase Policy`: Service requiring authentication.
    * `Submit Claim`: Extends to `Upload Documents` for evidence processing.

## 3. E-Shop System
**File:** `eShoop.png`

**Description:**
A comprehensive overview of an online shopping platform, identifying the roles of customers, administrators, and external payment services.

* **Actors:** Customer, Store Admin, Payment Gateway.
* **Key Use Cases:**
    * `Browse Catalog`: Public navigation.
    * `Checkout`: Includes `Calculate Total` and `Authenticate`.
    * `Apply Coupon`: Extends the `Checkout` process as an optional feature.
    * `Manage Inventory`: Restricted functionality for the Store Admin.

## 4. Medical Clinic System
**File:** `medical.png`

**Description:**
This diagram models a hospital management interface, focusing on patient-centric operations and data security.

* **Actors:** Patient, Clinic Database.
* **Key Use Cases:**
    * `Authenticate`: Strictly required before accessing personal records or making appointments.
    * `Make Appointment`: Extends to `Cancel Appointment`.
    * `View Medical Record`: Access requires prior authentication.
    * `Update Personal Info`: Direct interaction with the patient profile.

---

## Tools & Notations
* **Notation:** Standard UML 2.5 Use Case notation.
* **Relationships used:**
    * `Association`: Solid lines representing communication between actors and use cases.
    * `<<include>>`: Representing mandatory dependencies.
    * `<<extend>>`: Representing conditional or optional functional paths.

