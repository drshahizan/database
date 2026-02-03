# 🚗 Hasta Car Rental System Database Project 📊
<br>

> **Course**: SECP2523: Database (WBL)  
> **Session**: SEM I 2025/2026  
> **Section**: 02  
> **Lecturer**: PM Dr Mohd Shahizan Othman  
> **Stakeholder**: Hasta Travel & Tours Sdn. Bhd.  

---

## 🎡 Team SpinTheWheel
### Group Picture
![WhatsApp Image 2026-02-03 at 16 27 57](https://github.com/user-attachments/assets/d816b83b-deef-4a33-aa20-603057cd228c)

### Members
| Name | Matric ID | Role |
| :--- | :--- | :--- |
| **Chun Yao Ting** | A24CS0239 | Team Leader |
| **Evelyn Ang** | A24CS0068 | Member |
| **Mirza As-Siddiq Bin Tohari** | A24CS0112 | Member |
| **Muhammad Aliff Bin Helmi** | A24CS0272 | Member |

---

## 📖 Project Overview

This project focuses on the end-to-end analysis, design, and implementation of a centralized database system for **Hasta Travel & Tours Sdn. Bhd.**, a car rental service provider at Universiti Teknologi Malaysia (UTM).

The goal was to transition the company from a manual, fragmented workflow (WhatsApp, Excel, Whiteboard) to a streamlined, automated, and database-driven solution.

---

## 🔹 [Phase 1 – Project Proposal]() 

> **Phase 1** focuses on identifying the problems in the current manual system and proposing a digital solution.

### 🚩 Problem Statement
The current operation relies heavily on **manual methods**:
-   **Booking**: Handled via WhatsApp messages.
-   **Tracking**: Physical whiteboards for car availability.
-   **Records**: Handwritten forms and scattered Excel files.

**Key Issues**:
-   ❌ High risk of data redundancy and human error.
-   ❌ Inefficient booking & approval process.
-   ❌ Difficulty in tracking rental history and generating reports.

### 💡 Proposed Solution
A **Centralized Relational Database System** to:
-   ✅ Automate booking eligibility checks.
-   ✅ Enable real-time car availability tracking.
-   ✅ Securely store customer data and documents.
-   ✅ Generate automated sales and revenue reports.

**System Scope**:
-   **Customer Portal**: Registration, Booking, Payment, Profile Management.
-   **Staff Portal**: Approval, Car Management, Return Inspection.
-   **Admin Portal**: Analytics Dashboard, Staff Management.

---

## 🔹 [Phase 2 – Database Conceptual Design]()  

> **Phase 2** translates the requirements into a structured conceptual data model.

### 📐 Design Artifacts
-   **Data Flow Diagram (DFD)**: Mapped the flow of information between Customers, Staff, Admin, and the System processes (e.g., Manage Booking, Manage Payment).
-   **Entity Relationship Diagram (ERD)**: Defined key entities including `Users`, `Customers`, `Cars`, `Rentals`, `Payments`, `Vouchers`, and `Penalties`.
-   **Enhanced ERD (EERD)**: Implemented specialized subclasses for `Users` (into `Customer` and `Staff`) to optimize attribute inheritance.

### 📜 Business Rules Highlights
-   **Booking**: A car cannot be double-booked for overlapping time slots.
-   **Availability**: Cars enter a cooldown period (1 hour) after return for cleaning/inspection.
-   **Loyalty Program**: 1 Stamp per >12h booking; 3 Stamps = 1 Voucher.
-   **Penalties**: Late returns (>30 mins) incur RM50/hour charges.

---

## 🔹 [Phase 3 – Database Reporting & Implementation]()

> **Phase 3** involves the final logical design, normalization, and SQL implementation.

### ⚙️ Logical Design & Normalization
-   **Normalization**: All tables were normalized up to **Boyce-Codd Normal Form (BCNF)** to eliminate redundancy.
-   **Key Schemas**:
    -   `Rentals` table links `Customer`, `Car`, and `Staff`.
    -   `Payments` are strictly coupled with `Rentals`.
    -   `Vouchers` track usage status and validity.

### 🛠️ Implementation
-   **DDL (Data Definition Language)**: Created robust tables with integrity constraints (Primary Keys, Foreign Keys, `ON DELETE CASCADE`).
-   **DML (Data Manipulation Language)**:
    -   *Complex Queries*: Developed SQL for dashboard analytics (e.g., "Total Revenue Last 12 Months").
    -   *Triggers & Transactions*: Automated status updates (e.g., `Available` → `Rented` upon approval).

### 🖥️ Interface Design
Designed a modern web-based interface for:
-   **Customer**: Seamless booking flow, payment upload, and loyalty system.
-   **Staff**: Dashboard for "Pending Actions", and customer, rental, voucher, and car management.
-   **Admin**: Marketing Analytics Dashboard and Export Reporting in PDF or CSV.

---

<p align="center">
  <i>"Transforming operations from chaos to digital efficiency."</i>
</p>
