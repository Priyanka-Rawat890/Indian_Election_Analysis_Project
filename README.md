# 🗳️ Indian General Elections – SQL End-to-End Project  

---

## 🔍 Project Overview  
This project analyzes **Indian General Elections data** using SQL.  
The goal was to design queries that provide insights into **parties, alliances, states, and candidate performance**.  

---

## 🛠 Tools & Technologies Used  
- **SQL (MySQL / SQL Server)** – For querying and analysis  
- **Excel/CSV** – Raw dataset preparation  
- **Draw.io** – ERD diagram (optional, for schema visualization)  

---

## 📂 Project Deliverables  
- 🗂️ **SQL Queries:** [View SQL File](https://github.com/YourGitHubUsername/Indian-General-Elections-SQL-Project/blob/main/SQLQuery1.sql)  
- 🖼️ **ER Diagram (if available):** Add here  

---

## ✅ Key KPIs Analyzed  
- Seats won by each party  
- Alliance-wise performance  
- State-wise seat distribution  
- Winning margins by candidate  
- Top-performing candidates  

---

## 📊 Example Analyses in SQL  
```sql
-- Total seats won by each party
SELECT party, COUNT(seat_won) AS total_seats
FROM election_results
WHERE seat_won = 1
GROUP BY party
ORDER BY total_seats DESC;

-- Winning margin analysis
SELECT candidate, constituency, (votes_won - votes_runner_up) AS margin
FROM election_results
ORDER BY margin DESC;
