Banking System (OOP Case Study)
1. Project Overview:
This project implements a simple banking system using Object‑Oriented Programming (OOP) concepts.
It includes three core classes:

Account – manages account number and balance

Customer – stores customer information

Transaction – processes deposits and withdrawals

The purpose of this project is to practice OOP fundamentals and demonstrate how software design principles guide clean, maintainable code.

2. Software Design Principles Demonstrated
Encapsulation
Each class stores its own data internally:

Account keeps balance and account_number inside the object.

Customer stores name and its associated Account.

Transaction stores transaction details.

Access to these attributes happens only through methods such as deposit(), withdraw(), and display_balance().
This protects the internal state and prevents accidental modification.

Single Responsibility Principle (SRP)
Each class has one clear responsibility:

Account → handles money operations

Customer → represents a person with an account

Transaction → executes a deposit or withdrawal

This separation makes the system easier to understand and extend.

Abstraction
The user interacts with simple methods:

deposit(amount)

withdraw(amount)

display_balance()

They do not need to know how the balance is stored or updated internally.
This hides complexity and provides a clean interface.

Object Interaction (Composition)
The classes work together:

A Customer has an Account

A Transaction uses an Account to perform actions

This models real‑world banking behavior and shows how objects collaborate.

Loose Coupling
Customer and Transaction interact with Account only through its public methods.
They do not access internal variables directly.
This reduces dependency and makes future changes easier.

3. Thought Process and Design Reasoning
Why three classes?
Separating the system into Account, Customer, and Transaction keeps responsibilities clear.
It avoids mixing logic and makes the code easier to maintain.

Why methods instead of direct variable access?
Using methods like deposit() and withdraw() ensures:

Validation can be added later

Balance updates remain controlled

The internal structure of the class can change without affecting other classes

This is the essence of encapsulation.

Why call display_balance() inside Customer?
This demonstrates object interaction.
A customer does not manage money directly; their account does.

Why use a Transaction class?
It separates transaction logic from account logic.
This makes the system more modular and allows future extensions such as:

Transaction history

Different transaction types

Logging and auditing

4. Summary of Analysis
This banking system demonstrates key OOP principles:

Encapsulation protects data

SRP keeps classes focused

Abstraction hides complexity

Object interaction models real‑world behavior

Loose coupling makes the system flexible

The design is simple but effective, showing how OOP helps structure code in a clear and maintainable way.

5. Conclusion
This project serves as a foundational example of how software design principles guide the creation of clean, organized, and scalable code.
The structure, comments, and class interactions help others understand the reasoning behind the design and how OOP concepts are applied in practice

Inventory Item Management System
1. Project Overview
This project demonstrates a simple inventory‑management system using Object‑Oriented Programming (OOP) concepts.
It includes one main class:

InventoryItem – manages item creation, updates, storage, and display.

The goal is to practice OOP fundamentals and apply software‑design principles in a real‑world scenario.

2. Software Design Principles Demonstrated
Encapsulation
The class stores all inventory data internally:

item_counter tracks unique item IDs

inventory dictionary stores all items

Items can only be added, updated, or displayed through class methods.
This protects the internal state and prevents accidental modification.

Single Responsibility Principle (SRP)
Each method has one clear job:

add_inventory_item() → creates and stores a new item

calculate_total_value() → adds item + computes total value

update_inventory() → updates quantity and price

display_inventory_item() → shows item details

This separation makes the code easier to understand and maintain.

Abstraction
The class hides internal details and provides simple interfaces:

Users do not need to know how item IDs are generated

They simply call methods, and the class handles the logic internally

This keeps the system simple and user‑friendly.

Class Variables & Shared State
The project demonstrates how class variables can be used to maintain shared data:

item_counter ensures unique IDs

inventory stores all items in one central place

This models a real inventory system where all items belong to one shared store.

Object Interaction
A single object (system = InventoryItem()) manages all inventory operations:

Adding items

Updating items

Displaying items

This shows how objects coordinate tasks in an OOP system.

3. Thought Process and Design Reasoning
Why use class variables?
Inventory systems require shared data.
Using class variables ensures:

All items are stored together

IDs remain consistent

No duplicates occur

Why separate methods?
Each method handles one operation, making the system modular and easier to extend.

Why return item details?
Returning values allows future features such as:

Logging

Exporting inventory

Tracking changes

Why include user input?
This makes the system interactive and demonstrates how OOP can be used in real applications.

4. Summary of Analysis
This inventory system demonstrates key OOP principles:

Encapsulation protects inventory data

SRP keeps methods focused

Abstraction hides complexity

Class variables maintain shared state

Object interaction models real‑world behavior

The design is simple but effective, showing how OOP helps structure code in a clear and maintainable way.

5. Conclusion
This project is a practical example of how software‑design principles guide clean and organized code.
The structure, comments, and class interactions help others understand the reasoning behind the design and how OOP concepts are applied in practice.
