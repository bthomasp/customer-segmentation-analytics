# Customer Segment Revenue Analysis

## Overview
This project analyzes transactional ticket data to identify which customer segments generate the highest revenue per order.

The analysis reflects a common use case in media, advertising, and consumer analytics: understanding which audiences drive the most value to inform targeting, pricing, and strategic decision-making.

Analysis performed on a sample of transaction-level data (8,000 records) to simulate real-world analytical workflows.

## Approach
- Extracted and prepared transaction-level ticket data
- Aggregated to order-level metrics
- Joined with customer segmentation data
- Calculated revenue per order by segment
- Ranked segments based on performance

## Tools
- Python (pandas)
- PySpark (data preparation)
- SQL-style aggregations

## Key Insight
Segments such as "Tourist" and "VIP" generate the highest revenue per order, indicating strong opportunities for targeted marketing, premium pricing strategies, and audience prioritization.

## Why this matters
This type of analysis mirrors real-world use cases in:
- advertising performance measurement
- customer segmentation
- revenue optimization

## Example Output
Sample aggregated results (sorted by revenue per order):
| Segment | Total Revenue | Total Orders | Revenue per Order |
|--------|--------------|-------------|-------------------|
| Tourist | 140136.18 | 1019 | 137.52 |
| VIP | 139547.50 | 1019 | 136.95 |
| Unknown | 135985.40 | 997 | 136.39 |
| Group | 128233.64 | 952 | 134.70 |
| Student | 129816.97 | 971 | 133.69 |
| Local | 138935.73  | 1042 | 133.34 |

(Note: values based on sample dataset)

## Data Model
The analysis operates on two core datasets:
- Ticket events (transaction-level sales data)
- Customer dimension (segmentation attributes)

These are joined on customer_id to enable segment-level performance analysis.

