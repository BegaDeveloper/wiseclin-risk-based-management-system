# ⚕️ WiseClin – RBQM (Risk-Based Quality Management)

## 🚀 Introduction

**WiseClin RBQM** is a **Risk-Based Quality Management platform** developed for the **clinical research and healthcare sector in Spain**.
Its primary goal is to help research organizations and pharmaceutical companies **identify, assess, and manage risks proactively** throughout the entire **clinical trial lifecycle**.

The platform is designed to **ensure data integrity, patient safety, and regulatory compliance**, providing clinical teams with the visibility and control needed to make informed, data-driven decisions.

---

## 🧠 What the App Does

RBQM (Risk-Based Quality Management) is a key methodology in modern clinical trials, ensuring that potential risks are detected early and mitigated systematically.
The WiseClin platform digitizes this process, enabling research professionals to:

* 🧩 **Identify potential study risks** at planning and design phases.
* 📊 **Evaluate risk impact and probability** through scoring and visualization tools.
* 🧾 **Create and monitor risk mitigation plans** in real time.
* 🔄 **Track ongoing site quality and performance metrics.**
* 📡 **Generate regulatory-compliant reports** for auditors and sponsors.

By transforming manual spreadsheets and static workflows into a dynamic web system, WiseClin RBQM helps organizations **accelerate compliance and reduce operational errors** in complex clinical environments.

---

## 🧩 Technologies Used

| Layer               | Stack / Tools                                                      | Description                                                                          |
| ------------------- | ------------------------------------------------------------------ | ------------------------------------------------------------------------------------ |
| **Frontend**        | **Angular 17**, **RxJS**, **PrimeNg**, **NgRx**, **SCSS** | Built responsive, data-driven interfaces for risk analysis and monitoring workflows. |
| **Backend**         | **.NET / ASP.NET Core**                                            | Handled APIs, risk logic, and compliance workflows.                                  |
| **Database**        | **SQL Server**                                                     | Stored risk matrices, user configurations, and audit trails.                         |
| **Cloud / Hosting** | **Azure**                                                          | Deployed for high availability and healthcare-grade security.                        |

---

## 💻 My Role & Contributions

I worked as an **Angular Developer** on the WiseClin RBQM project, contributing to the development of **core frontend modules** that supported the risk evaluation and management process for clinical trials.

My focus was on building **intuitive, performance-optimized components** that allowed clinical researchers and QA teams to visualize, assess, and act on study risks quickly and efficiently.

Key contributions:

* Developed **dynamic, data-driven Angular components** for risk assessment dashboards and heat maps.
* Implemented **NgRx state management** to handle real-time updates to risk indicators and mitigation plans.
* Built **modular UI elements** (cards, charts, forms) following clean, reusable component design.
* Integrated **PrimeNg** for professional-grade UI consistency and accessibility.
* Collaborated with backend developers to connect Angular modules with **.NET Core APIs** for data exchange and report generation.
* Focused on **performance tuning**, ensuring low-latency UI updates even with complex datasets.

---

## ⚙️ Key Technical Highlights I Implemented

### 🧩 1. Dynamic Risk Matrix Visualization

One of my key tasks was to build a **dynamic risk evaluation matrix** that visualizes potential study risks based on their **impact and likelihood**.
The challenge was to render and update these matrices in real time as users entered new parameters.

I implemented:

* Reactive **RxJS streams** + Signals that listen for parameter changes.
* A **dynamic matrix component** that redraws color-coded cells (green/yellow/red) to represent current risk levels.
* **NgRx selectors** to manage real-time synchronization between user actions and the displayed risk matrix.

This resulted in a responsive, interactive, and intuitive risk visualization tool used daily by study monitors and QA teams.

---

### ⚙️ 2. Modular Risk Assessment Forms

Built **configurable Angular forms** for defining and editing risk parameters — such as severity, probability, and mitigation actions — using a shared schema-driven approach.

Each form was built with:

* Reactive Form Controls.
* Dynamic validation logic based on the type of risk.
* Role-based permissions for editing and approving risk data.

This allowed non-technical users (clinical leads, data managers) to configure assessments without developer input.

---

### ⚙️ 3. Data Consistency & Synchronization

Implemented **real-time synchronization** across multiple users editing the same risk data.
Used NgRx effects and RxJS subjects to broadcast updates, ensuring all users saw the latest risk states without needing to reload.

Example pattern:

```typescript
this.riskState$ = this.store.select(selectAllRisks).pipe(
  debounceTime(150),
  distinctUntilChanged(),
  shareReplay(1)
);
```

This pattern minimized redundant API calls and guaranteed **data consistency** across sessions.

---

## 🏁 Outcome

WiseClin RBQM became a **key platform for managing and monitoring clinical trial risks** in Spain, adopted by multiple research organizations for its compliance readiness, reliability, and user experience.
The Angular frontend played a critical role in transforming static, document-based risk tracking into a **real-time digital monitoring system**, improving transparency and auditability across all clinical operations.
