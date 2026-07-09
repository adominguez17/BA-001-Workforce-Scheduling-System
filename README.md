# BA-001 | Workforce Planning & Scheduling System

> Business Analytics Portfolio Series

Designed and implemented an automated workforce scheduling solution that improved operational planning, staffing visibility, and executive reporting for a workforce operating under continuous staffing requirements.

---
# Executive Summary

Designed and implemented a workforce planning and scheduling solution supporting a 350-person operational workforce operating under continuous staffing requirements.

The solution automated workforce scheduling by integrating employee data exported from Smartsheet into a centralized Microsoft Excel platform utilizing Power Query, advanced formulas, and automated forecasting. The system projected employee work rotations, generated annual scheduling forecasts, monitored staffing levels, and ensured contractual staffing requirements were consistently maintained.

By automating workforce planning, leadership gained advance visibility into employee rotations, staffing shortages, position coverage, and billing thresholds months in advance, significantly reducing manual scheduling efforts while improving operational planning and decision-making.

# 📊 Project Snapshot

| Category | Details |
|----------|---------|
| Role | Business Analyst / Solution Designer |
| Industry | Workforce Operations |
| Workforce Supported | 350+ Employees |
| Primary Tools | Excel, Power Query, Power BI |
| Project Type | Process Automation & Operational Reporting |
| Status | Production Implementation |

---

# Business Context

The organization managed approximately 350 operational employees working a 56-day on / 14-day off rotational schedule. Employee demographic information was maintained within Smartsheet by Human Resources, while scheduling activities were performed manually within a separate Excel workbook.

As workforce size increased, manually forecasting employee rotations, maintaining staffing levels, and ensuring contractual staffing obligations became increasingly complex. Leadership required greater visibility into workforce availability while ensuring staffing levels never dropped below required contractual minimums needed to satisfy client billing requirements and operational readiness.

# Business Problem

The existing scheduling process relied on manually exporting employee information from Smartsheet into a large Excel workbook used for workforce scheduling.

This manual process created several operational challenges:

- Annual scheduling forecasts required significant manual effort.
- Workforce rotations were difficult to visualize months in advance.
- Staffing shortages could occur without sufficient visibility.
- Position-level staffing requirements required continuous manual verification.
- Leadership lacked centralized reporting for workforce planning.
- Billing thresholds depended upon maintaining minimum active staffing levels at all times.

# Project Objectives

The project was designed to accomplish the following objectives:

- Automate the transfer of workforce data from Smartsheet into Excel.
- Forecast employee work rotations for the entire calendar year.
- Maintain contractual minimum staffing levels.
- Maximize billable workforce hours.
- Provide leadership with advance visibility into workforce availability.
- Monitor staffing coverage by shift and operational position.
- Reduce manual scheduling activities.
- Improve operational reporting and workforce planning.

# Business Rules & Constraints
The Workforce planning system was designed around several operational and contractual requirements.

### Operational Rules

- Support a workforce of approximately 350 employees.
- Enforce a 56-day on / 14-day off rotational schedule.
- Forecast workforce availability for the entire calendar year.
- Track staffing coverage by operational shift (A & B).
- Track staffing coverage by operational position.

### Contractual Constraints

- Maintain minimum staffing thresholds at all times.
- Maximize billable workforce availability.
- Prevent staffing levels from falling below contractual requirements.
- Support advance planning for employee leave rotations.
- Provide leadership with visibility into future staffing shortages.


# Business Decision Logic
The workforce planning engine evaluated each scheduling cycle against operational and contractual requirements before the schedule was considered acceptable.

```mermaid
flowchart TD

A[Import Employee Data]
A --> B[Generate Work Rotation]
B --> C[Calculate Annual Forecast]
C --> D[Validate Staffing by Shift]
D --> E[Validate Staffing by Position]

E --> F{Minimum Staffing Met?}

F -->|No| G[Adjust Schedule]
G --> B

F -->|Yes| H{Contract Staffing Threshold Met?}

H -->|No| G

H -->|Yes| I[Executive Dashboard]
I --> J[Leadership Reviews]
J --> K[Approve Workforce Plan]
```

# My Role 

I independently designed, developed, tested, and implemented the workforce scheduling solution from concept through production use.

Responsibilities included:

- Designing the overall workforce scheduling architecture.
- Designed the data integration workflow by transforming employee data exported from Smartsheet into a centralized workforce planning platform using Power Query.
- Developing Power Query transformations.
- Creating advanced Excel calculations supporting workforce forecasting.
- Designing scheduling logic for a 56-day on / 14-day off rotation.
- Building staffing validation tools to maintain contractual staffing requirements.
- Developing operational dashboards and reporting.
- Creating planning tools allowing leadership to forecast workforce availability months in advance.

# Solution Workflow

```mermaid
flowchart TD

A[HR Maintains Employee Records<br/>Smartsheet]

B[Export Employee Data]

C[Power Query<br/>Data Cleaning & Transformation]

D[Automated Workforce Planning Engine]

A --> B
B --> C
C --> D

D --> E[Annual Workforce Forecast]

D --> F[56-Day On<br/>14-Day Off Rotation]

D --> G[Position Staffing Validation]

D --> H[Shift A/B Coverage]

D --> I[Contract Staffing Threshold]

E --> J[Executive Dashboard]
F --> J
G --> J
H --> J
I --> J

J --> K[Leadership Planning]

K --> L[Operational Scheduling Decisions]
```


# System Architecture

```mermaid
flowchart TD
    A[Human Resources]
    B[Employee Data<br/>Smartsheet]
    C[Power Query]
    D[Workforce Planning Engine]
    E[Annual Forecast]
    F[Staffing Validation]
    G[Executive Dashboard]

    A --> B
    B --> C
    C --> D
    D --> E
    D --> F
    E --> G
    F --> G
```

# Technologies Used

| Technology | Purpose |
|------------|---------|
| Microsoft Excel | Workforce planning platform and scheduling engine |
| Power Query | Automated data import, transformation, and standardization |
| Advanced Excel Formulas | Workforce forecasting, staffing validation, and scheduling logic |
| Pivot Tables | Workforce reporting and operational summaries |
| Conditional Formatting | Staffing alerts and workforce visibility |
| Smartsheet | Employee demographic data source maintained by Human Resources |

# Key Features

- Automated workforce scheduling for approximately 350 employees.
- Forecasted employee work rotations across the entire calendar year.
- Supported a 56-day on / 14-day off rotational staffing model.
- Automated workforce data integration from Smartsheet exports.
- Maintained contractual minimum staffing requirements.
- Maximized billable workforce availability.
- Monitored staffing coverage by operational shift.
- Validated staffing levels by operational position.
- Forecasted employee leave months in advance.
- Improved organizational communication regarding upcoming workforce rotations.
- Produced operational dashboards and executive reporting.
- Reduced manual scheduling effort through workflow automation.

# Results

...

---

# Screenshots

(Images will go here later.)

---

# Lessons Learned

...

---

# Future Enhancements

...
