# ER Diagram Workshop – Submission Template

## Objective
To understand and apply ER modeling concepts by creating ER diagrams for real-world applications.

## Purpose
Gain hands-on experience in designing ER diagrams that represent database structure including entities, relationships, attributes, and constraints.

---

# Scenario A: City Fitness Club Management

**Business Context:**  
FlexiFit Gym wants a database to manage its members, trainers, and fitness programs.

**Requirements:**  
- Members register with name, membership type, and start date.  
- Each member can join multiple programs (Yoga, Zumba, Weight Training).  
- Trainers assigned to programs; a program may have multiple trainers.  
- Members may book personal training sessions with trainers.  
- Attendance recorded for each session.  
- Payments tracked for memberships and sessions.

### ER Diagram:
*Paste or attach your diagram here*  
![ER Diagram](er_diagram_fitness.png)

### Entities and Attributes

| Entity | Attributes (PK, FK) | Notes |
|--------|--------------------|-------|
|        |                    |       |
|        |                    |       |
|        |                    |       |
|        |                    |       |
|        |                    |       |

### Relationships and Constraints

| Relationship | Cardinality | Participation | Notes |
|--------------|------------|---------------|-------|
|              |            |               |       |
|              |            |               |       |
|              |            |               |       |

### Assumptions
- 
- 
- 

---

# Scenario B: City Library Event & Book Lending System

**Business Context:**  
The Central Library wants to manage book lending and cultural events.

**Requirements:**  
- Members borrow books, with loan and return dates tracked.  
- Each book has title, author, and category.  
- Library organizes events; members can register.  
- Each event has one or more speakers/authors.  
- Rooms are booked for events and study.  
- Overdue fines apply for late returns.

### ER Diagram:
*Paste or attach your diagram here*  
![ER Diagram](er_diagram_library.png)

### Entities and Attributes

| Entity | Attributes (PK, FK) | Notes |
|--------|--------------------|-------|
|        |                    |       |
|        |                    |       |
|        |                    |       |
|        |                    |       |
|        |                    |       |

### Relationships and Constraints

| Relationship | Cardinality | Participation | Notes |
|--------------|------------|---------------|-------|
|              |            |               |       |
|              |            |               |       |
|              |            |               |       |

### Assumptions
- 
- 
- 

---

# Scenario C: Restaurant Table Reservation & Ordering

**Business Context:**  
A popular restaurant wants to manage reservations, orders, and billing.

**Requirements:**  
- Customers can reserve tables or walk in.  
- Each reservation includes date, time, and number of guests.  
- Customers place food orders linked to reservations.  
- Each order contains multiple dishes; dishes belong to categories (starter, main, dessert).  
- Bills generated per reservation, including food and service charges.  
- Waiters assigned to serve reservations.

### ER Diagram:
<img width="1162" height="672" alt="Screenshot 2026-10-10 091249" src="https://github.com/user-attachments/assets/1b6b8739-9aa5-410f-bcb9-a0acbdec5de2" />


### Entities and Attributes

| Entity      | Attributes (PK, FK)                              | Notes                      |
| ----------- | ------------------------------------------------ | -------------------------- |
| Customer    | **Customer_ID (PK)**, Name, Phone                | Stores customer details    |
| Reservation | **Reservation_ID (PK)**, Date, Time, No_of_Guest | Stores reservation details |
| Order       | **Order_ID (PK)**, Date, Amount                  | Stores food order details  |
| Dish        | **Dish_ID (PK)**, Name, Category, Price          | Stores menu information    |
| Waiter      | **Waiter_ID (PK)**, Name, Contact                | Stores waiter details      |


### Relationships and Constraints

| Relationship                   | Cardinality | Participation | Notes                                                                   |
| ------------------------------ | ----------- | ------------- | ----------------------------------------------------------------------- |
| Customer — Makes — Reservation | 1:M         | Total         | One customer can make multiple reservations.                            |
| Reservation — Has — Order      | 1:M         | Total         | One reservation can include multiple orders.                            |
| Order — Contains — Dish        | M:N         | Total         | An order can contain many dishes, and a dish can appear in many orders. |
| Waiter — Serves — Reservation  | 1:M         | Total         | One waiter can serve multiple reservations.                             |


### Assumptions
Each reservation is assigned to one waiter.

Bills are generated from the total amount of ordered dishes.

A customer may place multiple orders during a reservation.

---

## Instructions for Students

1. Complete **all three scenarios** (A, B, C).  
2. Identify entities, relationships, and attributes for each.  
3. Draw ER diagrams using **draw.io / diagrams.net** or hand-drawn & scanned.  
4. Fill in all tables and assumptions for each scenario.  
5. Export the completed Markdown (with diagrams) as **a single PDF**
