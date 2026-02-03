# 🚘 Hasta Car Rental System
> **Streamlining Fleet Operations for Universiti Teknologi Malaysia (UTM)**

---

## 🏫 Project & Course Details
| Category | Information |
| :--- | :--- |
| **Course** | SECP2523: Database |
| **Session** | SEM I 2025/2026 |
| **Stakeholder** | Hasta Travel & Tours (Sdn. Bhd.) |


---

## 🖐️ Team Gimme5
**"High-Performance Solutions for Modern Problems"**

| Member Name | Matric ID |
| :--- | :--- |
| **Gwee Zi Ni** | A24CS0078 |
| **Michelle Ho Chia Xin** | A24CS0110 |
| **Lee Jia Yee** | A24CS0260 |
| **Tay Xin Ying** | A24CS0200 |
| **Kalaitharan A/L Palanyvelu** | A24CS0091 |

---

## 🚀 Project Overview

**The Problem (As-Is):**
Hasta Travel & Tours currently relies on a fragmented manual system involving **WhatsApp**, **physical whiteboards**, and **Excel spreadsheets**. This leads to:
* ⏳ **Slow Confirmations:** Manual availability checks cause booking delays 
* 📉 **Data Redundancy:** Staff must re-enter data across multiple platforms (Driveo, Excel, Wahdah)
* ❌ **Human Error:** Manual calculation of fines, late fees, and fuel shortages is prone to mistakes 
* 🚫 **Disconnected Blacklists:** No real-time verification of blacklisted users during the booking conversation 

**The Solution (To-Be):**
We developed a **web-based Car Rental System** powered by a centralized **MySQL** database. This system automates the rental lifecycle, ensures real-time vehicle tracking, and integrates financial reporting for top management.

---

## 📂 Project Milestones

### 📍 Phase 1: System Proposal
**Focus:** *Feasibility Study & Requirement Analysis*

We conducted a comprehensive analysis of the current business processes to identify pain points and propose a digital solution.
* **Core Modules Identified:** User Management, Vehicle Inventory, Booking Engine, Payment Gateway, and Reporting.
* **Feasibility:** Confirmed technical viability using open-source technologies (HTML, PHP, MySQL).



---

### 📐 Phase 2: Conceptual Design
**Focus:** *ERD Modeling & Business Rules*

* **Entity Relationships:** Designed a robust ERD connecting Users, Vehicles, and Bookings.
* **Business Logic:** Defined constraints for "Minimum 1-hour rental" , "30-day document expiry alerts", and "Loyalty Stamp accumulation".

---

### 💻 Phase 3: Logical Design & Implementation
**Focus:** *Normalization, Schema Optimization & SQL Deployment*

We translated our conceptual model into a fully normalized database schema ready for deployment.

#### 🔧 Database Optimization
* **Normalization:** Applied **3NF (Third Normal Form)** to eliminate transitive dependencies (e.g., separating `Colleges`, `Faculties`, and `Pricing Tiers` into distinct tables)
* **Integrity:** Validated against **BCNF (Boyce-Codd Normal Form)** to ensure every determinant is a candidate key.
* **Data Dictionary:** Documented 20+ entities including `inspections`, `fines`, and `maintenance_logs`.

#### ⚡ Key Technical Features
* **Automated Triggers:** System automatically updates vehicle status to *'Unavailable'* upon booking confirmation.
* **Digital Inspections:** `inspections` table supports JSON storage for damage photos and fuel level verification.
* **Dynamic Pricing:** Implemented `pricing_rules` and `pricing_tiers` for flexible hourly rate calculations.



---

## ⚙️ System Modules & Features

| Module | Key Capabilities |
| :--- | :--- |
| **👤 User Management** | Secure login via Matric/Staff ID, digital document verification (IC/License), and automated **Blacklist Checks** . |
| **🚗 Vehicle Fleet** | [Real-time tracking of availability, maintenance logs, and automated alerts for **Road Tax/Insurance Expiry**. |
| **📅 Booking Engine** | Interactive calendar for reservations, minimum 1-hour rental logic, and automated conflict detection . |
| **💳 Payments & Fines** | Supports QR/Transfer proofs, automated deposit refund tracking, and distinct logic for **Fines & Penalties** . |
| **🎁 Loyalty & Rewards** | Automated stamp accumulation (1 stamp per 3+ hours) and voucher redemption system. |
| **📊 Reporting** | Generates financial profit/loss reports and demographic insights by Faculty/College for Top Management. |

---

<p align="center">
  <strong>Developed with ❤️ by Team Gimme5</strong><br>
  Universiti Teknologi Malaysia
</p>
