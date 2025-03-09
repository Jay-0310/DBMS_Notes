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

## 3. Data Models
A **Data Model** defines how data is structured and manipulated in a DBMS. The major types include:
- **Relational Model**: Uses tables (relations) with rows (tuples) and columns (attributes). This is the most widely used model.
- **Entity-Relationship (E-R) Model**: Graphical representation of entities and relationships.
- **Object-Based Data Models**: Extends the relational model with object-oriented concepts.
- **Semi-Structured Data Models**: Used for XML and NoSQL databases.
- **Older Models**: Network and hierarchical models.

---

## 4. Database Languages
DBMS provides specialized languages for defining and manipulating data:
- **DDL (Data Definition Language)**: Defines schema and structure (e.g., `CREATE TABLE`).
- **DML (Data Manipulation Language)**: Retrieves and modifies data (e.g., `SELECT`, `INSERT`, `UPDATE`).
- **Query Languages**:
  - **Relational Algebra** (theoretical foundation for queries)
  - **SQL (Structured Query Language)**: The standard language for interacting with relational databases.

---

## 5. Structured Query Language (SQL)
SQL is the most widely used database language and includes:
- **Data Definition**: `CREATE`, `ALTER`, `DROP`.
- **Data Manipulation**: `SELECT`, `INSERT`, `UPDATE`, `DELETE`.
- **Transaction Control**: `COMMIT`, `ROLLBACK`, `SAVEPOINT`.
- **Access Control**: `GRANT`, `REVOKE`.

SQL can be embedded in higher-level languages (e.g., Java, Python) through APIs like JDBC and ODBC.

---

## 6. Database Design
Database design involves structuring the data to ensure efficiency, consistency, and scalability. It has two main stages:
- **Logical Design**: Identifies the entities, attributes, and relationships. Determines the schema structure.
- **Physical Design**: Determines the storage structure, indexing, and access methods for efficient query processing.

### Design Approaches
1. **Entity-Relationship (E-R) Modeling**: Graphically represents entities and relationships.
2. **Normalization**: Eliminates redundancy and ensures data integrity.

---

## 7. Database Architecture & Components
A DBMS consists of multiple components that work together:
- **Storage Manager**: Manages database files, indexing, and access.
- **Query Processor**: Translates queries into low-level instructions.
- **Transaction Manager**: Ensures ACID (Atomicity, Consistency, Isolation, Durability) properties.
- **Concurrency Control**: Handles multiple users accessing data simultaneously.

### Transaction Management
- A **transaction** is a set of operations performed as a single unit.
- Ensures **atomicity** (all-or-nothing execution), **consistency**, **isolation** (no interference between transactions), and **durability** (data remains safe after a failure).

---

## 8. Database Users & Roles
DBMS is used by different types of users:
- **Database Administrators (DBA)**: Manage access, security, backups, and performance tuning.
- **Application Programmers**: Develop database-driven applications.
- **End Users**: Execute queries and retrieve information.

---

## 9. Conclusion
A **Database Management System (DBMS)** is essential for handling large-scale data efficiently. It overcomes the limitations of traditional file systems by providing:
- **Better data integrity**
- **Security and controlled access**
- **Efficient concurrent access**
- **Data independence**

By understanding the fundamentals of DBMS, we can design robust, scalable, and secure data storage solutions for modern applications.
