README.md

1. Activity Diagram
This diagram illustrates the operational workflow of the purchase process, from the perspective of user actions and system logic. It visualizes the step-by-step path a user takes:

Process Flow: Starts with browsing/searching, moves to product details, and handles the "Add to Cart" logic (including stock checking).

Decision Points: It clearly maps the conditional paths, such as checking if an item is in stock ([Yes] or [No]) and verifying if the payment was successful ([Yes] or [No]).

Non-functional Requirements: The box on the right explicitly defines constraints the system must adhere to, such as response time (NF-1.1), SSL encryption for payments (NF-2.1), and BCrpyt hashing for passwords (NF-2.2).

2. Class Diagram
This is a structural diagram that defines the static architecture of the E-Shop system. It shows the entities (classes) and how they relate to one another:

Core Entities: It identifies the primary objects in the system: Customer, Product, Shopping Cart, Authenticator, and Order.

Relationships: It uses UML notation to show associations (e.g., Customer browses Product), composition (the diamond shape connecting Product to Shopping Cart), and dependencies.

Encapsulation: For each class, it defines specific attributes (e.g., productID, price) and methods (e.g., reduceStock(), calculateTotal()), serving as a blueprint for the underlying code.

3. Sequence Diagram
This represents the dynamic behavior of the system, showing how different components interact over time during specific processes.

Interaction Flow: It details the "Add to Cart" and "Checkout" processes, mapping exactly which component (Web Application, Product Service, Cart Service, Database, Payment Gateway) communicates with which, and in what order.

Technical Steps: It tracks the sequence of events, such as checking stock in the database (steps 2-4) and the payment gateway interaction (steps 16-17).

Requirement Mapping: It explicitly references functional requirements (REQ-1.1 and REQ-1.2), showing exactly when these requirements are fulfilled during the execution flow.

4. State Diagram
This diagram describes the lifecycle of an order within the system. It tracks the various states an order transitions through from creation to completion:

States: It starts at the Cart (Active) state and follows a specific path through Checkout, Payment Processing, Order Confirmed, Shipped, and Delivered.

Transitions: It captures the logic for state changes (e.g., Submit order, Payment success, Ship order).

Exceptional States: It also accounts for failure and alternative paths, such as Payment Failed (which loops back to checkout) or order Cancelled and Returned scenarios.

5. Use Case Diagram
This diagram defines the functional scope and the relationship between users and the system features:

Actors: It identifies the three primary actors interacting with the E-Shop: Customer, Store Admin, and the external Payment Gateway.

Use Cases: It lists the core functionalities, such as Browse Catalog, Add to cart, Checkout, and Manage inventory.

Relationships: It uses standard UML include and extend relationships to show dependencies (e.g., Checkout includes Authenticate and calculate Total; Apply coupon extends Checkout).