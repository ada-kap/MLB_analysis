# ⚾ SQL Analysis of MLB Players and Their Schools

This project was created as part of the Udemy course **“SQL for Data Analysis: Advanced SQL Querying Techniques”**. The analysis focuses on historical data from Major League Baseball (MLB). 

🙋‍♀️ **About the Author**

Aspiring data analyst transitioning from a different career background. Passionate about turning real-world data into actionable insights. This project is part of a growing data analytics portfolio aimed at showcasing practical SQL skills.

## 🎯 Project Goal

- Analyze the relationship between MLB players and the schools they attended.
- Practice advanced SQL querying techniques using real-world relational data.
- Build an analytical project portfolio as part of a career transition into **data analytics**.

---

## 🗃️ Dataset Overview

The analysis is based on two main tables:

📊 Data Table: schools
| Column   | Type    | Description                                |
|----------|---------|--------------------------------------------|
| playerID | TEXT    | Unique identifier of a player              |
| schoolID | TEXT    | Unique identifier of a school              |
| yearID   | INTEGER | Year when the player attended the school   |

📊 Data Table: school_details
| Column    | Type    | Description                                 |
|-----------|---------|---------------------------------------------|
| schoolID  | TEXT    | Unique school identifier                    |
| name_full | TEXT    | Full name of the school                     |
| city      | TEXT    | City where the school is located            |
| state     | TEXT    | State (for US-based schools)                |
| country   | TEXT    | Country where the school is located         |

📊 Data Table: salaries
| Column   | Type | Description           |
| -------- | ---- | --------------------- |
| yearID   | INT  | Year of the salary    |
| teamID   | TEXT | Team identifier       |
| lgID     | TEXT | League identifier     |
| playerID | TEXT | Player identifier     |
| salary   | INT  | Salary value (in USD) |

📊 Data Table: players
| Column          | Type | Description                                  |
| --------------- | ---- | -------------------------------------------- |
| playerID        | TEXT | Unique player ID                             |
| birthYear       | INT  | Year of birth                                |
| birthMonth      | INT  | Month of birth                               |
| birthDay        | INT  | Day of birth                                 |
| debut\_date     | DATE | Date of first MLB game                       |
| finalGame\_date | DATE | Date of last MLB game                        |
| nameFirst       | TEXT | First name                                   |
| nameLast        | TEXT | Last name                                    |
| ...             | ...  | Additional biographical columns omitted here |

---

⚙️ Tools & Technologies
- MySQL
- SQL client: DBeaver
- Data source: Provided via Udemy course dataset
- GitHub

## 🔍 Key Analytical Questions

1. How many schools produced MLB players in each decade?
   _Purpose: Analyze the growth or decline of schools contributing to MLB players over time._

2. What are the top 5 schools that produced the most MLB players? 
   _Purpose: Identify the most influential schools in player development._

3. For each decade, which were the top 3 schools producing the most players?
   _Purpose: Understand shifts in dominance among schools over different eras.
   
5. Return the top 20% of teams in terms of average annual spending
   _Goal: Identify the biggest spenders among teams.

7. For each team, show the cumulative sum of spending over the years
   _Goal: Visualize long-term team investment.

9. Return the first year that each team’s cumulative spending surpassed 1 billion USD
   _Goal: Understand financial growth over time.

10. How many players are in the table?
    _Goal: Get basic scope of the dataset.

12. For each player, calculate age at debut, age at final game, and career length (in years). 
    _Goal: Analyze career duration across MLB history.
