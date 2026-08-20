# Deloitte Australia — Data Analytics Job Simulation

A client-style data analytics case study completed through the **Deloitte Australia Data Analytics Job Simulation on Forage**.

The simulation focused on transforming operational and employee compensation data into structured, business-facing analysis using **Tableau and Excel**.

---

## Business Problems

The simulation covered two analytical tasks:

### 1. Operational Downtime Analysis

Analyze machine telemetry data to understand potential downtime across Daikibo factories and identify the device types associated with the highest downtime.

**Key analytical steps**
- Imported telemetry data into Tableau
- Created a calculated downtime measure from machine status
- Compared potential downtime across factories
- Analyzed downtime by device type
- Built an interactive dashboard where factory selection filters device-level analysis

## Dashboard Preview

![Daikibo Downtime Analysis](Task-1-Operational-Analytics/dashboard.png)

**Key finding:** Daikibo Factory Seiko recorded the highest potential downtime at **480 minutes**, with LaserWelder accounting for the recorded downtime in the filtered device-level view.

[Explore Task 1 →](Task-1-Operational-Analytics/README.md)

---

### 2. Equality Score Classification

Classify employee compensation equality scores into three business-defined categories:

| Equality Score | Classification |
|---:|---|
| -10 to +10 | Fair |
| -20 to -11 or +11 to +20 | Unfair |
| Below -20 or above +20 | Highly Discriminative |

The classification was implemented in Excel using a reproducible formula rather than manually assigning categories.

[Explore Task 2 →](Task-2-Equality-Analysis/README.md)

---

## Tools

- **Tableau** — data visualization and interactive dashboarding
- **Microsoft Excel** — business-rule classification and spreadsheet analysis

---

## Analytical Approach

The work followed a simple analyst workflow:

**Business requirement → Data preparation → Metric/rule definition → Analysis → Visualization → Business interpretation**

The emphasis was on making the analysis reproducible, understandable, and aligned with the stated business requirements.

---

## Deliverables

- Tableau downtime dashboard
- Completed equality classification workbook
- Task-level methodology and findings
- Deloitte Australia / Forage completion certificate

---

## Certificate

The completion certificate is included in the `Certificate/` directory.

---

## Disclaimer

This repository contains my work and documentation from a Deloitte Australia job simulation hosted by Forage. Deloitte and Forage names, trademarks, and simulation materials remain the property of their respective owners. This repository should not be interpreted as evidence of employment with Deloitte or work performed for a Deloitte client.
