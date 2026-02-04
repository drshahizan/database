# 🚗 Hasta Car Rental System Database Project 📊

> **Course**: SECP2523 – Database (WBL)  
> **Session**: Semester I 2025/2026  
> **Section**: 02  
> **Lecturer**: PM Dr. Mohd Shahizan Othman  
> **Industry Stakeholder**: Hasta Travel & Tours Sdn. Bhd.

---

## 👥 Team QueryCrew

### Group Members
| No. | Name | Matric Number | Role |
|:--:|:--|:--|:--|
| 1 | **Kavinesh Reddy A/L Gopalakrishnan** | A24CS0092 | Team Leader |
| 2 | **Muhammad Al-Hakimi Haikal Bin Romi Sabihin** | A24CS0271 | Member |
| 3 | **Haritz Haykal Bin Nazrul Hisham** | A24CS0250 | Member |
| 4 | **Niveethitha A/P Pandia Rajan** | A24CS0148 | Member |

---

## 📖 Project Overview

This project involves the analysis, design, and implementation of a **centralized database system** for **Hasta Travel & Tours Sdn. Bhd.**, a car rental service operating within Universiti Teknologi Malaysia (UTM).

The company previously relied on **manual and fragmented processes**, such as WhatsApp messaging, handwritten records, and Excel spreadsheets. This project aims to transform those processes into a **structured, reliable, and database-driven system** to improve operational efficiency and data accuracy.

---

## 🔹 Phase 1 – Project Proposal

Phase 1 focuses on identifying the problems in the existing manual workflow and proposing a suitable database-based solution.

### 🚩 Problem Statement
The current car rental operation faces several challenges:
- Bookings are managed through WhatsApp messages  
- Car availability is tracked using physical whiteboards  
- Records are stored across handwritten forms and Excel files  

**Key Issues**:
- High risk of data redundancy and human errors  
- Inefficient booking and approval process  
- Difficulty in tracking rental history and generating reports  

### 💡 Proposed Solution
A **Centralized Relational Database System** to:
- Automate booking validation and approval  
- Enable real-time car availability tracking  
- Securely store customer data and documents  
- Support automated reporting and analytics  

**System Scope**:
- **Customer Module**: Registration, booking, payment, and profile management  
- **Staff Module**: Booking approval, car management, and inspections  
- **Admin Module**: Staff management, analytics, and reporting  

---

## 🔹 Phase 2 – Database Conceptual Design

Phase 2 translates system requirements into a structured conceptual data model.

### 📐 Design Deliverables
- **Data Flow Diagram (DFD)** showing data flow between users and system processes  
- **Entity Relationship Diagram (ERD)** defining core entities such as Customer, Staff, Car, Booking, Payment, and Voucher  
- **Enhanced ERD (EERD)** applying specialization and generalization for different user roles  

### 📜 Key Business Rules
- A car cannot be double-booked for overlapping time periods  
- Cars require a cooldown period after return for inspection  
- Loyalty stamps are awarded based on rental duration  
- Late returns incur penalty charges  

---

## 🔹 Phase 3 – Logical Design & Implementation

Phase 3 focuses on logical design, normalization, and SQL implementation.

### ⚙️ Logical Design & Normalization
- All relations were normalized up to **Third Normal Form (3NF) / BCNF**  
- Data redundancy and dependency issues were eliminated  
- Logical ERD was derived from the conceptual design and business rules  

### 🛠️ Database Implementation
- **DDL**: Tables created with Primary Keys, Foreign Keys, UNIQUE, and NOT NULL constraints  
- **DML**: SQL statements written for insertion, updates, deletion, and reporting  
- **Integrity Control**: Referential integrity and cascading rules enforced  

---

## 🎯 Conclusion

This project demonstrates how a well-designed database system can improve efficiency, accuracy, and scalability in a real-world car rental operation. By replacing manual workflows with a centralized database, Hasta Travel & Tours Sdn. Bhd. can achieve better data management and operational control.

<p align="center">
  <i>"Designing structured data for smarter operations."</i>
</p>
