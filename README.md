# 📊 COVID-19 Database Insights and Trends Analysis with SQL

## Overview

This project is a comprehensive data exploration of global COVID-19 data using SQL. It involves cleaning, analyzing, and generating insights from a dataset containing information about COVID-19 cases, deaths, vaccinations, and population statistics across over 100 countries and multiple continents. The project provides a robust foundation for visualization and dashboarding by creating meaningful views and aggregated insights.

---

## 📁 Dataset

The dataset contains information on:

- **COVID-19 Cases**: Total and daily cases per country
- **Deaths**: Total and daily deaths
- **Vaccinations**: Vaccination counts and trends
- **Population**: Country-wise population for percentage calculations

Data Source: Public COVID-19 dataset (e.g., Our World in Data)

---

## 🔧 Skills & Techniques Used

- SQL Joins
- CTEs (Common Table Expressions)
- Temp Tables
- Window Functions
- Aggregate Functions
- Data Type Conversion
- View Creation for Visualization

---

## 🧪 Key Analyses

### 📍 General Exploration
- Filtered for valid country-level data using `continent IS NOT NULL`
- Explored population, total cases, deaths, and new cases over time

### 📉 Death Percentage by Country
Calculated the likelihood of dying from COVID-19 in each country:
```sql
(total_deaths / total_cases) * 100
