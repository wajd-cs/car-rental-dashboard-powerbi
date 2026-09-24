<div align="center">

# Car Rental Dashboard (Power BI)

**An interactive Power BI dashboard analyzing a car rental company's contracts, rental revenue, booking status, car types, and branches across Saudi cities.**

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Dashboard](https://img.shields.io/badge/Dashboard-8A2BE2?style=for-the-badge)
![Data Analysis](https://img.shields.io/badge/Data_Analysis-4479A1?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Complete-2EA44F?style=for-the-badge)

</div>

---

## Table of Contents
- [Overview](#overview)
- [What the Project Contains](#what-the-project-contains)
- [How I Built It](#how-i-built-it)
- [Key Metrics](#key-metrics)
- [Insights](#insights)
- [Dashboard](#dashboard)
- [Skills Demonstrated](#skills-demonstrated)
- [Author](#author)

---

## Overview

A one-page Power BI report for a fictional car rental company. It answers three business questions at a glance: how many contracts were signed and how much they are worth, which car types bring in the most revenue, and how contracts are distributed across branches and booking statuses.

It continues my data analysis learning path after the [Hospital Patients Dashboard](https://github.com/wajd-cs/hospital-dashboard-powerbi), applying the same Power BI workflow to a new business domain.

## What the Project Contains

A Power BI report built on rental contract records (data in Arabic), covering:

| Field | Description |
|---|---|
| Contract | One row per rental contract |
| Car Type | SUV, Sedan, Pickup |
| Branch | Riyadh, Jeddah, Makkah, Madinah, Dammam, Khobar, Abha |
| Booking Status | Completed, In Progress, Cancelled |
| Rental Value | Contract value in SAR |

The dashboard includes:

- **2 KPI cards** — number of rental contracts and total rental value
- **3 charts** — contracts by branch (column), rental value by car type (bar), and booking status distribution (pie)
- **2 slicers** — filter the whole report by car type or branch

## How I Built It

```mermaid
flowchart LR
    A[1. Import Data] --> B[2. Prepare in Power Query]
    B --> C[3. KPI Cards]
    C --> D[4. Charts]
    D --> E[5. Slicers]
    E --> F[6. Design & Layout]
```

**1. Loaded the data** — 15 rental contract records, also available in `car-rental-data.xlsx`.

**2. Prepared it in Power Query** — defined the data type of every column (text for IDs and categories, whole number for rental value) so counts and sums calculate correctly.

**3. Built KPI cards** — a count of contracts and a sum of rental value as the headline numbers.

**4. Created charts**, choosing the type that fits each question:

| Chart | Type | Question |
|---|---|---|
| Contracts by branch | Column | Which branches are busiest? |
| Rental value by car type | Bar | Which car types generate the most revenue? |
| Booking status | Pie | What share of bookings are completed, ongoing, or cancelled? |

**5. Added slicers** for car type and branch, so one selection filters every card and chart on the page.

**6. Designed the layout** — KPIs on top, charts in the center, and slicers on the side, with a consistent navy-blue theme.

## Key Metrics

| Metric | Value |
|---|---|
| Rental contracts | 15 |
| Total rental value | ~15K SAR |
| Completed bookings | 10 (66.7%) |
| In progress | 3 (20%) |
| Cancelled | 2 (13.3%) |
| Branches | 7 |

## Insights

- **SUVs generate the most revenue** — nearly as much as Sedans and Pickups combined — making them the company's most valuable category.
- **Riyadh and Jeddah are the busiest branches** with 3 contracts each, while Khobar has the fewest with 1.
- **Two-thirds of bookings were completed**, and about 13% were cancelled — a rate worth tracking, since cancellations mean lost revenue and idle cars.

*Note: with only 15 records, this project focuses on demonstrating Power BI techniques and dashboard design rather than statistically significant findings.*

## Dashboard

![Dashboard](screenshots/dashboard.png)

## Skills Demonstrated

- **Power Query** — preparing data with correct headers and types
- **Aggregations** — counting contracts and summing revenue across different dimensions
- **Data Visualization** — matching chart types to business questions
- **Interactive Filtering** — slicers that filter the entire report
- **Dashboard Design** — clear layout with a consistent visual theme
- **Business Thinking** — turning booking and revenue data into operational observations

## Author

**Wajd Alluhaibi**
Computer Science Student | Data Analysis & Software Development

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/wajd-al-luhaibi-9194a1396)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:wajdalharbics@gmail.com)
