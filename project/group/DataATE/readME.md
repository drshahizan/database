# 🚗 Hasta Travel Vehicle Rental Management System (DataATE)
> **A Comprehensive Database Transformation Project**

---

## 🏛️ Course Information
| Category | Details |
| :--- | :--- |
| **Course** | SECP2523: Database (WBL) |
| **Session** | SEM I 2025/2026 |
| **Section** | 02 |
| **Lecturer** | PM Dr. Mohd Shahizan Othman |
| **Stakeholder** | Encik Alif (Hasta Travel & Tours Sdn. Bhd.) |

---

## 🛰️ Team DataATE
### 📸 Group Presence
![Team Photo](https://github.com/user-attachments/assets/86143b45-db57-4d78-aa88-5f21bb427ab6)


### 👥 Member Directory
| Name | Matric ID | Role |
| :--- | :--- | :--- |
| **Angela Ngu Xin Yi** | A24CS0226 | Team Leader |
| **Gavenesh A/L Batumalai** | A24CS0076 | Member |
| **Tan Xin Tian** | A24CS0198 | Member |
| **Teoh Xin Yee** | A24CS0307 | Member |
| **Toh Shee Thong** | A24CS0309 | Member |

---

## 🛠️ Project Roadmap & Deliverables

### 📍 [MILESTONE 01] : SYSTEM PROPOSAL
**Objective:** *Deconstructing the "As-Is" manual flow to architect a digital "To-Be" solution.*

📂 **Access Document:** [DataATE_P1_Proposal.pdf](./DataATE_P1_Proposal.pdf)

**THE CHALLENGE**
* **Booking Delays:** WhatsApp dependency creates response lag and communication gaps.
* **Data Inconsistency:** Scattered records across Paper and Excel files drive frequent human error.
* **Double Bookings:** Manual whiteboard tracking lacks real-time updates, risking overlaps.
* **Compliance:** Current manual methods struggle to meet modern LHDN e-Invoicing requirements.

**THE INNOVATION**
* `Real-time Availability` — Interactive calendar for instant fleet tracking and reservation.
* `Automated Logic` — Instant mathematical calculation for late penalties and fuel shortages.
* `Identity Vault` — Secure digital portal for verifying IC, Matric cards, and Licenses.
* `Loyalty Engine` — Automated stamp-based system to reward frequent customers.

---

### 📐 [MILESTONE 02] : CONCEPTUAL ARCHITECTURE
**Objective:** *Translating business requirements into high-fidelity technical blueprints.*

📂 **Access Document:** [DataATE_P2_ConceptualDesignReport.pdf](./DataATE_P2_ConceptualDesignReport.pdf)



[Image of a database Entity Relationship Diagram]


**DESIGN ARTIFACTS**
* **DFD Mapping:** Established 8 core processes ranging from Login/Registration to Deposit Withdrawal.
* **Enhanced ERD:** Developed a specialized **User Hierarchy** (distinguishing Admin vs. Customer roles).
* **Data Dictionary:** Rigorous documentation of data types, field lengths, and integrity constraints.

**⚙️ CORE SYSTEM LOGIC**
* 🛡️ **Verification Rule** | User profiles must be flagged as `Verified` by the administrator before the system enables the booking module.
* 🛠️ **Fleet Integrity** | Any vehicle marked with a `Maintenance` status is automatically excluded from the real-time availability pool.
* ⏱️ **Grace Period** | A strictly enforced 30-minute window for returns; exceeding this triggers an automated **RM50/hour** penalty.
* 🎖️ **Loyalty Logic** | Rentals exceeding **9 hours** earn 1 stamp; accumulation of 3 stamps triggers a system-generated reward.

---

### 💻 [MILESTONE 03] : IMPLEMENTATION & REPORTING
**Objective:** *Logical design normalization, relational mapping, and full SQL deployment.*

📂 **Access Document:** [DataATE_P3_LogicalDesignReport.pdf](./DataATE_P3_LogicalDesignReport.pdf)



#### 🏗️ THE LOGICAL FOUNDATION
* **Normalization:** Optimized the system schema up to **Boyce-Codd Normal Form (BCNF)** to eliminate all potential data redundancy and update anomalies.
* **Relational Schema:** Created a centralized integration hub connecting `Rentals`, `Cars`, `Payments`, and `Vouchers` for seamless data flow.
* **Asset Tracking:** Engineered detailed `Pickups` and `Returns` tables designed to capture precise vehicle condition reports and digital image paths for transparency.

#### ⚡ TECHNICAL EXECUTION
* **DDL Layer:** Successfully deployed **14 core relational tables** featuring strict Primary Key and Foreign Key constraints to maintain referential integrity.
* **DML Layer:** Engineered complex **Join Queries** specifically for the Managerial Dashboard to provide real-time Revenue and Fleet Health analysis.
* **Automated Triggers:** Scripted advanced database triggers to automate status notifications and initiate deposit refund processing upon vehicle return.

---

<p align="center">
  <i>"Optimizing efficiency, one query at a time."</i>
  <br><br>
  <strong>DataATE © 2026</strong>
</p>
