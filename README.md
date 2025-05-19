# DataAnalytics-assessment-

# OVERVIEW
This project contains solutions to four SQL-based business analysis tasks, each addressing a real-world data problem.


## Question 1 – High-Value Customers
**Approach towards work 
Joined user data with savings and investment tables to filter only users with at least one funded plan in each category. Aggregated deposits and sorted them.

--Challenge in the work process 
Initial issues with missing status column were resolved by checking schema and using is_funded.


## Question 2 – Transaction Frequency Analysis
**Approach towards work  
Calculated monthly average transactions per user and used a CASE statement to categorize frequency levels.

--Challenge in the work process 
Assumed transaction_date existed and represented a valid transaction — fallback plan included simulating frequency via transaction count over distinct months.


## Question 3 – Account Inactivity Alert
**Approach towards work 
Queried both savings and investment accounts using DATEDIFF to identify records with no activity in over 365 days. Combined results using UNION.

 --Challenge in the work process 
Ensured that date formats were compatible with DATEDIFF and confirmed consistent date columns.


## Question 4 – Customer Lifetime Value (CLV)
**Approach towards work 
Computed tenure from date_joined, counted all transactions, and used the provided CLV formula with average transaction value.

--Challenge in the work process 
Avoided division by zero with NULLIF, and confirmed profitability formula logic.

Updated Readme
