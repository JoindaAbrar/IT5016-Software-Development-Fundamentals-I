Simple Banking System (OOP Case Study)
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
