<div align="center">



<!-- Replace the line below with your own banner image URL -->
<img src="https://github.com/drshahizan/database/raw/1b6a01bf600c7f214d18bfbab8838f961ccf59ad/project/group/404NotFound/hastalogo.png" 
     alt="Banner" 
     width="400"/>

<h1>🚗 Hasta Vehicle Rental Booking System</h1>

<p><em>Every record has a reason. Every table has a purpose.</em></p>

📘 **Course** : SECP2523 DATABASE &nbsp; | &nbsp; 📅 **Session** : SEM I 2025/2026 &nbsp; | &nbsp; 🔢 **Section** : 02

👨‍🏫 **Lecturer** : Prof. Madya. Ts. Dr. Mohd Shahizan bin Othman &nbsp; | &nbsp; 🏢 **Stakeholder** : Hasta Travel & Tours Sdn. Bhd.

<br/>

<img src="https://img.shields.io/badge/MySQL-00758F?style=for-the-badge&logo=mysql&logoColor=fff" />
<img src="https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=fff" />
<img src="https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=fff" />
<img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=fff" />
<img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=fff" />
<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=000" />

<br/><br/>

🗃️ **11 Normalized Tables** &nbsp; | &nbsp; 📦 **5 Modules** &nbsp; | &nbsp; ✅ **16 Use Cases**

</div>

---

## 👥 Team 404NotFound

<div align="center">
<img src="https://github.com/drshahizan/database/raw/1b6a01bf600c7f214d18bfbab8838f961ccf59ad/project/group/404NotFound/404NotFound%20Picture.jpeg" 
     alt="Group Photo" 
     width="700"/>

</div>

<br/>

| 👤 | Name | 🎫 Matric ID | ⚙️ Role |
| :---: | :--- | :---: | :--- |
| 🏆 | **Parthiv Gunalan** | A24CS0178 | Team Leader |
| 💻 | **Heng Zhi Qiang** | A24CS0081 | Member |
| 💻 | **Leong Jia Ling** | A24CS0104 | Member |
| 💻 | **Hong Jia Bao** | A24CS0251 | Member |
| 💻 | **Lee Pei Yuan** | A24CS0262 | Member |

> 🏢 **Stakeholder Representative:** Encik Alif Firdaus *(Owner, Hasta Travel & Tours Sdn Bhd)* — interviewed across **6 sessions** from Oct 2025 – Jan 2026.

---

## 📖 Project Overview

Hasta Travel & Tours is a **UTM-exclusive** 🎓 car rental service that previously ran on a patchwork of WhatsApp, Google Sheets, physical whiteboards, and Drive Wahdah — none of them connected.

This project builds a **centralized relational database** that replaces all of that with one structured, queryable, and auditable system powering the full rental lifecycle. The old way was scattered across WhatsApp chats, whiteboard markers, Excel files, and manual notes — the new way is a clean, normalized MySQL database with real-time availability, automated enforcement, and proper reporting.

---

## 🗂️ Phase 1 — Initial Proposed System

> 🎯 *Stakeholder interviews · Problem identification · System scope*

- 📝 Documented the **full existing manual workflow** through **6 interview sessions** with the business owner
- 🔍 Pinpointed core pain points: duplicate bookings, lost receipts, unenforced blacklists, zero real-time availability
- 🎯 Defined **8 mission objectives** & clear boundaries — GPS tracking, insurance APIs, and direct bank integration are explicitly out of scope
- ⚙️ Proposed a **Laravel + MySQL** stack with 3 role-based user types: **Customer · Staff · Admin**

---

## 📐 Phase 2 — Conceptual Database Design

> 🎯 *Requirement translation · Local ERDs → Global ERD · Data Dictionary*

- 🧩 Built **5 module-level ERDs** (Rewards, Fleet, User, Booking, Reporting), then merged into one **Global Conceptual ERD**
- 📊 Mapped out **6 core entities** — User, Staff, Car, Booking, Reward, and CarImage — along with **8 relationships** with full cardinality rules. For example, a User can make many Bookings, each Booking reserves exactly one Car, and a Booking can optionally apply one Reward voucher.

- 📄 Documented **transaction requirements** for every module — entries, updates, deletions, and queries
- ✅ Verified the Global ERD for cross-module conflicts and redundancies

---

## 🧮 Phase 3 — Logical Design & Implementation

> 🎯 *Logical ERD · Normalization · Full DDL & DML · Interface Design*

- 📝 Refined the conceptual model into a **logical schema** with precise data types, keys, lengths, and constraints
- 📐 Normalized **step-by-step** all the way to **BCNF** — starting from 6 tables in UNF, splitting out JSON arrays in 1NF to get 9 tables, then resolving transitive dependencies in 3NF to arrive at the final **11 tables**.

- 💾 Delivered **full DDL & DML** for all **16 use cases** — registration, booking flows, fleet management, reporting, and loyalty redemption
- 🖥️ Designed complete **interface mockups** for both customer and admin portals

---

## 📦 The 5 Modules at a Glance

| # | 📦 Module | ⭐ Symbol | 📌 Covers |
| :---: | :--- | :---: | :--- |
| 1 | User Management | 👤 | Register, Login, Docs Upload, Verification, Profile |
| 2 | Car Rental Booking | 🚗 | Book, Pay, Pickup, Return, Cancel, History |
| 3 | Fleet Management | 🔧 | Add / Edit / Status control of vehicles |
| 4 | Reporting | 📊 | Monthly & weekly revenue, booking analytics |
| 5 | Loyalty & Rewards | 🏷️ | Points tracking, voucher redeem & apply |
