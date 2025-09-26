# Olist E-commerce Data Analysis using SQL
This project showcase exploratory and business-focused data analysis on the Olist E-commerce Dataset using SQL. The goal is to extract actionable insights on sales performance, customer behavior, and operational efficiency.

Datasets can be found in below link 
https://www.kaggle.com/olistbr/brazilian-ecommerce.

# DB Schema 
<img width="639" alt="Screen Shot 2025-07-06 at 12 30 28" src="https://github.com/user-attachments/assets/3f70bac1-6c04-417c-ad2b-e55c74058cce" />

# Project Objectives 
- Explore dataset using SQL
- Answer key business questions through structured queries
- Uncover trends in geolocation, delivery times, and customer satisfaction
- Provide insights to help optimize market place operations

# Tools & Technologies
- SQL (Standard SQL, compatible with PostgreSQL/BigQuery)
- Jupyter Notebook
- Olist Public Dataset

# Business Questions Answered
- How do delivery times vary by state? 
- Which sellers generate the most sales?
- What patterns exist in customer reviews?
- What is the geographic distribution or orders and customers?

# Key Findings 

## Delivery times by state

Delivery performance varies by geography: states in the Southeast (e.g., São Paulo—SP, Minas Gerais—MG, Rio de Janeiro—RJ) generally see faster delivery due to denser logistics networks, while parts of the North/Northeast (e.g., Amazonas—AM, Pará—PA, Roraima—RR) tend to have longer lead times because of distance and transport constraints. In practice, you’ll see average delivery times a couple of days faster in the Southeast than in the North/Northeast, with wider tails for remote areas.

## Patterns in customer reviews

By state, the notebook shows some of the highest average scores in AP (~4.18), AM and PR (~4.18), and SP (~4.17), and the lowest in AL (~3.75), MA (~3.76), SE (~3.81), PA (~3.85), and CE (~3.85).

## Geographic distribution of orders and customers

Customers — and thus orders — are heavily concentrated in the Southeast:

The notebook’s output shows São Paulo (SP) alone accounts for about 37.47% of top 5 states regarding total turnover, with Rio de Janeiro (RJ) next at roughly 13%.

The remaining flow is spread across MG, RS, PR, and other states, with progressively smaller shares as you move away from the core Southeast corridor.

# Recommendation
## Reviews (lift scores without gaming them)

Root-cause drill-down: For the five lowest-score states, break reviews by late/on-time, seller, carrier, and category; fix the top offenders first.


