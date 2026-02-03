# 🚘 Hasta Car Rental System
> **Streamlining Fleet Operations for Universiti Teknologi Malaysia (UTM)**

---

## 🏫 Project & Course Details
| Category | Information |
| :--- | :--- |
| **Course** | SECP2523: Database |
| **Session** | SEM I 2025/2026 |
| **Stakeholder** | Hasta Travel & Tours (Sdn. Bhd.) |
| **Focus** | Digital Transformation & Centralized Database Management |

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
[cite_start]Hasta Travel & Tours currently relies on a fragmented manual system involving **WhatsApp**, **physical whiteboards**, and **Excel spreadsheets**[cite: 1316, 1326]. This leads to:
* [cite_start]⏳ **Slow Confirmations:** Manual availability checks cause booking delays [cite: 1328-1329].
* [cite_start]📉 **Data Redundancy:** Staff must re-enter data across multiple platforms (Driveo, Excel, Wahdah)[cite: 1330].
* [cite_start]❌ **Human Error:** Manual calculation of fines, late fees, and fuel shortages is prone to mistakes [cite: 1335-1336].
* [cite_start]🚫 **Disconnected Blacklists:** No real-time verification of blacklisted users during the booking conversation [cite: 1339-1341].

**The Solution (To-Be):**
[cite_start]We developed a **web-based Car Rental System** powered by a centralized **MySQL** database [cite: 1317-1318]. [cite_start]This system automates the rental lifecycle, ensures real-time vehicle tracking, and integrates financial reporting for top management[cite: 1322, 1402].

---

## 📂 Project Milestones

### 📍 Phase 1: System Proposal
**Focus:** *Feasibility Study & Requirement Analysis*

We conducted a comprehensive analysis of the current business processes to identify pain points and propose a digital solution.
* [cite_start]**Core Modules Identified:** User Management, Vehicle Inventory, Booking Engine, Payment Gateway, and Reporting [cite: 1304-1305].
* [cite_start]**Feasibility:** Confirmed technical viability using open-source technologies (HTML, PHP, MySQL)[cite: 1373].

📄 **[View Phase 1 Report](DB%20Project%20Report%20P1.pdf)**

---

### 📐 Phase 2: Conceptual Design
**Focus:** *ERD Modeling & Business Rules*

* [cite_start]**Entity Relationships:** Designed a robust ERD connecting Users, Vehicles, and Bookings[cite: 1947].
* [cite_start]**Business Logic:** Defined constraints for "Minimum 1-hour rental" [cite: 1437][cite_start], "30-day document expiry alerts" [cite: 1431][cite_start], and "Loyalty Stamp accumulation"[cite: 1416].

---

### 💻 Phase 3: Logical Design & Implementation
**Focus:** *Normalization, Schema Optimization & SQL Deployment*

[cite_start]We translated our conceptual model into a fully normalized database schema ready for deployment [cite: 26-27].

#### 🔧 Database Optimization
* [cite_start]**Normalization:** Applied **3NF (Third Normal Form)** to eliminate transitive dependencies (e.g., separating `Colleges`, `Faculties`, and `Pricing Tiers` into distinct tables)[cite: 28, 226].
* [cite_start]**Integrity:** Validated against **BCNF (Boyce-Codd Normal Form)** to ensure every determinant is a candidate key[cite: 29].
* [cite_start]**Data Dictionary:** Documented 20+ entities including `inspections`, `fines`, and `maintenance_logs`[cite: 93, 117, 121, 129].

#### ⚡ Key Technical Features
* [cite_start]**Automated Triggers:** System automatically updates vehicle status to *'Unavailable'* upon booking confirmation[cite: 45].
* [cite_start]**Digital Inspections:** `inspections` table supports JSON storage for damage photos and fuel level verification[cite: 122, 124].
* [cite_start]**Dynamic Pricing:** Implemented `pricing_rules` and `pricing_tiers` for flexible hourly rate calculations[cite: 141, 143].

📄 **[View Phase 3 Report](DB%20Project%20Report%20P3.pdf)**

---

## ⚙️ System Modules & Features

| Module | Key Capabilities |
| :--- | :--- |
| **👤 User Management** | [cite_start]Secure login via Matric/Staff ID, digital document verification (IC/License), and automated **Blacklist Checks** [cite: 42-43]. |
| **🚗 Vehicle Fleet** | [cite_start]Real-time tracking of availability, maintenance logs, and automated alerts for **Road Tax/Insurance Expiry**[cite: 44, 1428]. |
| **📅 Booking Engine** | [cite_start]Interactive calendar for reservations, minimum 1-hour rental logic, and automated conflict detection [cite: 46, 1437-1438]. |
| **💳 Payments & Fines** | [cite_start]Supports QR/Transfer proofs, automated deposit refund tracking, and distinct logic for **Fines & Penalties** [cite: 48-49, 1457]. |
| **🎁 Loyalty & Rewards** | [cite_start]Automated stamp accumulation (1 stamp per 3+ hours) and voucher redemption system[cite: 97, 1416]. |
| **📊 Reporting** | [cite_start]Generates financial profit/loss reports and demographic insights by Faculty/College for Top Management[cite: 50, 1463]. |

---

<p align="center">
  <strong>Developed with ❤️ by Team Gimme5</strong><br>
  Universiti Teknologi Malaysia
</p>
