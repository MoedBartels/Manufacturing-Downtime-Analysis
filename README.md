# Manufacturing-Downtime-Analysis

### Soda Bottling Production Line | Excel | Power Query | Power BI

## Project Overview

This project analyzes productivity and downtime across a soda bottling production line.

The analysis focuses on four key business questions:

1. What is the current line efficiency?
2. Are any operators underperforming?
3. What are the leading factors for downtime?
4. Do operators experience particular types of downtime classified as operator error?

The project was designed as a practical Excel → Power Query → Power BI workflow, with the dashboard focused on answering the core questions rather than attempting to analyze every available dimension of the dataset.

## Key Findings

| Metric | Result |
|---|---:|
| Line Efficiency | **64.02%** |
| Production Batches | **38** |
| Total Production Time | **3,858 mins / 64.3 hrs** |
| Total Downtime | **1,388 mins / 23.1 hrs** |
| Average Downtime per Batch | **36.53 mins** |
| Operator-Error-Classified Downtime | **776 mins / 12.9 hrs** |

### Main Findings

- **Machine adjustment** was the largest downtime factor at **332 minutes**.
- **Machine failure** accounted for **254 minutes**.
- **Inventory shortage** accounted for **225 minutes**.
- Together, these three factors represented approximately **58.4% of total recorded downtime**.
- **Cola** recorded the highest total downtime at **771 minutes (12.9 hours)**.
- Operator efficiency was relatively closely grouped across the four operators.
- Among factors classified as Operator Error, **machine adjustment** was the largest category overall, while **batch change** was particularly prominent for Mac.

## Operator Error Classification

The dataset includes an `Operator Error` classification for downtime factors.

This classification applies to the **downtime factor**, not to the individual operator. A factor marked `Yes` indicates that the dataset categorizes that type of downtime as an operator error; it does not establish that a particular operator was personally responsible for causing the event.

The operator-error analysis was therefore separated from the overall operator downtime analysis.

## Tools & Workflow

**Excel**
- Initial data preparation
- Power Query data cleaning and transformation

**Power BI**
- Data modelling
- Calculated fields
- KPI calculations
- Interactive dashboard
- Operator and product filtering
- Downtime analysis

## Dashboard

The Power BI dashboard provides an interactive view of:

- Overall line efficiency
- Total production and downtime
- Downtime by factor
- Downtime by flavor
- Operator efficiency
- Overall operator downtime patterns
- Operator-error-classified downtime

## Scope

The analysis was intentionally focused on the four questions recommended by Maven Analytics.

The dataset supports additional analysis across products, flavors, batch volumes and other dimensions, but these were not included in the main dashboard in order to keep the analysis focused and concise.

## Limitations

- The analysis identifies patterns in the available data but does not establish causality.
- Total downtime by flavor does not account for differences in production volume.
- The Operator Error classification does not establish individual operator responsibility.
- The dataset does not contain financial information, so the financial cost of downtime could not be quantified.

## Full Report

A detailed written report containing the methodology, findings, limitations and further areas for investigation is included in this repository.
