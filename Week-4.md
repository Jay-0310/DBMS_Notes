# Week 4 Lecture Material: Relational Database Design

---

## **Module 16: Relational Database Design/1**
### **Week 03 Recap**
- **Module 11:** Advanced SQL (Accessing SQL from a programming language, Functions, Triggers)
- **Module 12:** Formal Relational Query Languages (Relational Algebra, Tuple & Domain Relational Calculus)
- **Module 13-15:** Entity-Relationship Model (E-R Diagrams, Relational Schema, Extended Features)

### **Module Objectives**
- Identify features of a good relational design
- Understand First Normal Form (1NF)
- Learn about Functional Dependencies

### **Key Topics**
1. **Features of Good Relational Design**
   - Atomic Domains and First Normal Form (1NF)
   - Functional Dependencies
   - Schema Decomposition & its impact on redundancy

2. **First Normal Form (1NF)**
   - Atomicity of attributes
   - Non-atomic values leading to redundancy
   - Multi-valued attributes & composite attributes

3. **Functional Dependencies**
   - Definition and importance
   - Superkeys & Candidate keys
   - Lossless decomposition of schemas
   
---

## **Module 17: Relational Database Design/2**
### **Objectives**
- Understanding schema decomposition for efficient design
- Introduction to Functional Dependency Theory

### **Key Topics**
1. **Boyce-Codd Normal Form (BCNF)**
   - Condition: If **α → β**, then α is a superkey
   - Example: `inst_dept(ID, name, salary, dept_name, building, budget)` where `dept_name → building, budget` violates BCNF
   
2. **BCNF Decomposition Process**
   - Identifying functional dependencies causing violations
   - Decomposing into smaller relations while preserving constraints

3. **Dependency Preservation & 3rd Normal Form (3NF)**
   - 3NF ensures dependency preservation when BCNF is not possible
   - Ensuring decomposed relations still maintain constraints

---

## **Module 18: Relational Database Design/3**
### **Objectives**
- Algorithms for Functional Dependencies
- Characterizing Lossless Join Decomposition
- Understanding Dependency Preservation

### **Key Topics**
1. **Functional Dependency Theory**
   - Closure of a set of functional dependencies
   - Armstrong’s Axioms (Reflexivity, Augmentation, Transitivity)

2. **Canonical Cover & Minimal Sets**
   - Eliminating redundant dependencies
   - Identifying extraneous attributes

3. **Candidate Keys & Super Keys**
   - Finding candidate keys using functional dependencies
   - Prime vs Non-Prime attributes

### **Practice Problems**
- Checking if a dependency follows from a set.
- Finding candidate keys & superkeys.
- Determining prime/non-prime attributes.

---

## **Summary**
- Importance of Normalization (1NF, 3NF, BCNF).
- Functional dependencies and their role in schema design.
- Decomposing schemas while preserving integrity.
