JAVA FX BOOKSTORE APPLICATION
COE 528 – Object Oriented Engineering Analysis and Design

--------------------------------------------------

PROJECT OVERVIEW

This project is a desktop Bookstore Application developed using JavaFX and NetBeans.
The application allows customers to browse and purchase books while earning and redeeming reward points, and allows store owners to manage books and customers.

The system is designed using object-oriented principles and applies the State Design Pattern to manage customer status changes.

--------------------------------------------------

SYSTEM ACTORS

1. Customer
- Logs into the bookstore application
- Browses available books
- Purchases books using money or reward points
- Earns points for purchases
- Redeems points
- Logs out

2. Owner
- Logs into the system as an administrator
- Manages books (add and delete)
- Manages customers (add and delete)
- Logs out

--------------------------------------------------

MAIN USE CASE: BUY BOOKS

Use Case Name: Buy Books
Primary Actor: Customer

ENTRY CONDITIONS
- Customer enters the bookstore application
- Customer logs in with correct credentials

FLOW OF EVENTS
1. Customer selects the number of books to purchase
2. Customer chooses whether to buy the books using money or redeem reward points
3. The system displays a new screen showing:
   - Total cost
   - Current reward points
   - Customer status
   - Logout option
4. The system completes the transaction and removes the purchased books from inventory

EXIT CONDITION
- Customer successfully purchases the selected book(s)

--------------------------------------------------

DESIGN PATTERN USED

STATE DESIGN PATTERN

The State Design Pattern is used to manage the customer’s status and behavior.

Customers earn points when purchasing books.
Customer status is determined by total points:
- Silver Status: fewer than 1000 points
- Gold Status: 1000 points or more

Because points and status change frequently, the system uses a State interface with concrete states:
- SilverState
- GoldState

The Customer class holds a reference to the current state.
This allows the customer’s status to change dynamically at runtime without using complex conditional statements.

Benefits of this design include:
- Improved readability
- Increased flexibility
- Easier maintenance
- Cleaner object-oriented design

--------------------------------------------------

TECHNOLOGIES USED

- Java
- JavaFX
- NetBeans IDE
- Object-Oriented Design Patterns

--------------------------------------------------

RUNNING THE APPLICATION

1. Open NetBeans
2. Load the Bookstore Application project
3. Ensure the project is using JDK 8 or JDK 11
4. Clean and Build the project
5. Run the application from NetBeans

--------------------------------------------------

PROJECT DOCUMENTATION

- Project report
- Use-case diagram
- Design pattern rationale
- System behavior description

--------------------------------------------------

AUTHORS

Cheran Balakrishnan
Tejveer Sidhu
Kevin Bhawan

COE 528 – Bookstore Application Project

--------------------------------------------------
