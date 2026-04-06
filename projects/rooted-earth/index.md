---
title: "RootedEarth Analytics – SQL & Business Intelligence"
description: "End-to-end retail analytics project using relational database design, SQL, and Power BI."
date: 2026-03-10
draft: false
tags: ["SQL", "Data Analysis", "Database Design", "Business Intelligence"]

_build:
  list: never
  render: always
---

## Overview

Built an end-to-end data analytics solution simulating a multi-location retail business across **10 locations** and **400+ transactions**.

This project combines **relational database design**, **SQL analysis**, and **Power BI visualization** to transform raw transactional data into actionable business insights.

---

## Database Design & Architecture

Designed a **normalized relational database schema (3NF)** to ensure data integrity and eliminate redundancy. The system supports complex relationships across **9 core entities**, including Customers, Orders, Products, and Locations.

![RootedEarth Schema](/images/projects/schema.png)

*Relational schema illustrating primary and foreign key relationships.*

---

## Data Analytics Layer

Developed **17+ SQL queries** to extract meaningful business insights from transactional data.

**Key Technical Implementations:**

- **Relational Joins:** Combined transactional and reference tables to produce clear, business-readable outputs  
- **Aggregations:** Used `SUM`, `COUNT`, and `GROUP BY` to analyze performance across time and locations  
- **Performance Optimization:** Applied indexing on high-traffic columns such as `OrderDate` and `LocationID` to improve query efficiency  

---

## Power BI Dashboard

This dashboard translates structured data into clear, visual insights for quick performance analysis.

**Interactive Sales Performance Overview**

![RootedEarth Sales Dashboard](/images/projects/rooted_earth_sales.png)

---

## Key Business Insights

- Generated **$4.1M in total revenue**, providing a high-level performance overview  
- Sales trends show consistent growth with noticeable seasonal peaks  
- A small group of products drives a disproportionate share of total revenue  
- Downtown location significantly outperforms other stores in overall sales  

---

## Key Outcome

This project demonstrates the ability to design a relational database, perform business-focused SQL analysis, and translate data into actionable insights through professional dashboarding.

---

## GitHub Repository

[View Full SQL Scripts](https://github.com/indiya88/rootedearth-database)