# Database Management Systems (Week 1 Notes)

## 1. Introduction to DBMS
A **Database Management System (DBMS)** is a software system that provides systematic storage, retrieval, and management of data in an organized manner. It serves as an interface between the user and the database, ensuring data integrity, security, and efficient access.

### Why Databases?
Databases are essential for managing structured and unstructured data in various applications, including:
- **Banking**: Transactions, account management, fraud detection.
- **Airlines**: Flight reservations, ticketing, and schedules.
- **Universities**: Student registration, course enrollment, grading.
- **E-commerce**: Order tracking, inventory management, recommendation systems.
- **Manufacturing**: Production planning, inventory control, supply chain management.
- **Human Resources**: Employee records, payroll, tax deductions.

### Drawbacks of File Systems
Before the emergence of DBMS, file systems were used for data storage, but they had several drawbacks:
- **Data Redundancy & Inconsistency**: Multiple copies of the same data lead to inconsistency and storage inefficiency.
- **Difficulty in Data Access**: Retrieving specific data required custom programs.
- **Data Isolation**: Different formats in multiple files made integration difficult.
- **Integrity Problems**: Ensuring constraints (e.g., balance > 0) was challenging.
- **Atomicity Issues**: Failure during a transaction could leave the database in an inconsistent state.
- **Concurrent Access Problems**: Multiple users accessing data simultaneously could lead to conflicts.
- **Security Issues**: Controlling access to sensitive information was difficult.

---

## 2. DBMS Abstraction Levels
To manage data efficiently, DBMS follows **three levels of abstraction**:
- **Physical Level**: Describes how data is stored physically in files and disks.
- **Logical Level**: Defines what data is stored and the relationships between data.
- **View Level**: Provides different perspectives of the database for different users, ensuring security and ease of access.

### University Database Example
A university database may include:
- **Entities**: Students, courses, instructors.
- **Relationships**: Enrollment, course assignments.
- **Operations**: Adding students, assigning grades, generating reports.

---
