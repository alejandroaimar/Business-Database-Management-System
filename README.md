# Business Database Management System

## Overview

This project involves the design and implementation of a relational database management system for "El Corte Maestro", a barbershop that operates as both a commercial establishment and a barber school. The solution replaces manual and semi-manual processes with a structured digital system capable of managing appointments, customers, payments, services, and the academic organization of 50 students distributed across 5 study groups.

The database was built using **MySQL 8.4.8**, with a normalized schema of **11 interconnected tables** and **over 500 real-world data records**, ensuring data consistency, integrity, and efficient querying for business decision-making.

---

## Objectives

- Design a relational database to centralize barbershop operations.
- Eliminate scheduling conflicts through unique constraints.
- Track customer information and complete visit history.
- Implement payment processing across multiple methods.
- Organize 50 students into 5 structured study groups.
- Enable data-driven decisions through business intelligence queries.

---

## Business Context

"El Corte Maestro" started as a traditional barbershop and expanded into a barber school model. The business currently operates with 3 instructors, 50 students, and 5 study groups organized by schedule.

### Problem Identified

Information management remained manual or semi-manual. Appointments were scheduled through WhatsApp, leading to double-booking and no availability control. Service records were kept in spreadsheets or physical notebooks, resulting in lost customer history. Payments were recorded on paper, causing accounting errors. There was no structured system to track student performance or organize study groups.

---

## Methodology

### 1. Database Design

The design process began with an Entity-Relationship model to identify entities, attributes, and relationships. The initial model was refined through multiple iterations to eliminate unnecessary tables and incorporate new requirements such as study groups and appointment status. The final schema was normalized to Third Normal Form (3NF) to eliminate redundancies and ensure data consistency.

### 2. Implementation

The database was implemented using MySQL 8.4.8. Primary and foreign keys were established to maintain referential integrity. Referential actions such as `ON DELETE CASCADE`, `ON DELETE SET NULL`, and `RESTRICT` were applied to control data behavior. ENUM data types were used for predefined values such as barber type and day of the week. Unique constraints were applied to prevent double-booking.

### 3. Data Population

Realistic test data was generated to validate the database structure. Customer names, contacts, and appointments were created with the assistance of AI tools. Service prices were researched from real barbershops. Payment methods were selected based on common practices in the Mexican market.

### 4. Business Intelligence

Ten business intelligence queries were developed to extract actionable insights from the database. These include revenue analysis, customer segmentation, service popularity, peak hours, staff performance, and occupancy rates.

---

## Technologies Used

- **MySQL 8.4.8** – Database engine.
- **SQL** – Data definition and query language.
- **Draw.io** – Entity-Relationship diagram design.
- **DeepSeek** – Data generation.
- **ChatGPT** – Debugging and conceptual support.

---

## Automation Implemented

- **Stored Procedure:** Displays all appointments for a given date.
- **Function:** Counts total appointments per customer.
- **View:** Summarizes barber performance metrics.
- **Trigger:** Validates email format before inserting new customers.

---

## Database Concepts Applied

- Entity-Relationship Modeling
- Relational Database Design
- Database Normalization (1NF → 2NF → 3NF)
- Primary and Foreign Keys
- Referential Integrity (CASCADE, SET NULL, RESTRICT)
- ENUM Data Types
- Composite Primary Keys
- Stored Procedures
- Functions
- Views
- Triggers
- Business Intelligence Queries
- Subqueries and Joins

---

## Results

The project provides:

- Fully normalized database schema (3NF).
- 11 interconnected tables.
- 500+ customer records.
- 514 appointment records.
- 15 services across 3 specialties.
- 53 barbers (3 instructors + 50 students).
- 5 structured study groups.
- Business intelligence queries for data-driven decisions.
- Automated features for operational efficiency.

---

## Project Structure

```text
Business-Database-Management-System/

├── sql/
│   └── 01_schema.sql

├── documentation/
│   └── Database_Project_Report.pdf

├── images/
│   └── ER_Diagram.png

├── README.md
└── LICENSE

```

---

## Author

**Alejandro Aimar y compañeros de la carrera**

Actuarial Science Student | Finance & Risk Management Enthusiast
