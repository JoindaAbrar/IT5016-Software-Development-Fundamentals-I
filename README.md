# IT5016-Software-Development-Fundamentals-I
Simple Banking System – OOP Case Study
Overview:
This project is a simple banking system designed to demonstrate fundamental Object‑Oriented Programming (OOP) concepts such as:

Encapsulation

Abstraction
Single Responsibility Principle (SRP)
Object Interaction
Basic class design
The system includes three main classes:
Account – manages account number and balance
Customer – stores customer information
Transaction – processes deposits and withdrawals
Software Design Principles Demonstrated:
1. Encapsulation
Each class stores its own data internally.
For example, the Account class keeps balance private to the object and exposes methods (deposit, withdraw) to modify it safely.
2. Single Responsibility Principle (SRP)
Each class has one clear purpose:
Account → manages money
Customer → represents a person with an account
Transaction → handles transaction logic
This separation improves readability and maintainability.
3. Abstraction
The user interacts with simple methods like:
deposit(amount)
withdraw(amount)
display_balance()
They do not need to know how the balance is stored or updated internally.
4. Object Interaction
Objects collaborate in a realistic way:
A Customer has an Account
A Transaction uses an Account to perform actions
This models real‑world banking behavior.
5. Loose Coupling
Customer and Transaction interact with Account only through its public methods.
This reduces dependency and makes the system easier to extend.
Code Comments and Explanation:
The code includes meaningful comments explaining:
Why each class exists
How OOP principles are applied
Where improvements can be made
Why certain design choices matter
These comments help readers understand the thought process behind the design.
Possible Improvements:
To enhance the system further:
Add transaction history
Validate negative amounts
Avoid executing logic inside constructors
Use enums for transaction types
Add error handling and logging

Conclusion
This simple banking system is an effective demonstration of OOP fundamentals.
It shows how classes interact, how responsibilities are separated, and how abstraction simplifies user interaction.
The comments and structure make the code easy to understand, extend, and maintain
