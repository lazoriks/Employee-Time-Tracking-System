# Employee-Time-Tracking-System
Employee Time Tracking System - Simple Version
==============================================

1. System Requirements
----------------------

Functional Requirements:
1. Add an employee.
2. Employee marks time of arrival (check-in).
3. Employee marks time of leaving (check-out).
4. Administrator views list of employees.
5. Administrator views time records.

Non-Functional Requirements:
1. System must be simple to use.
2. Data must be stored reliably.
3. Fast response time.
4. Support multiple users.

2. Use Cases
------------

UC1: Add Employee
Actor: Admin
Steps:
 1. Open "Add Employee"
 2. Enter name
 3. Save

UC2: Check-In
Actor: Employee
Steps:
 1. Press "Check-In"
 2. System stores timestamp

UC3: Check-Out
Actor: Employee
Steps:
 1. Press "Check-Out"
 2. System stores timestamp

UC4: View Employees
Actor: Admin
Steps:
 1. Open employees list
 2. View employees

UC5: View Time Records
Actor: Admin
Steps:
 1. Open time records
 2. View all check-in and check-out entries

3. Identified Classes
---------------------

Class Employee:
 - id: int
 - name: String

Class TimeRecord:
 - id: int
 - employeeId: int
 - checkIn: DateTime
 - checkOut: DateTime

Relationship:
 Employee 1 --- * TimeRecord