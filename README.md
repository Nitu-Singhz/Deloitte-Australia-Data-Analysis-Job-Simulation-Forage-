# Deloitte-Australia-Data-Analysis-Job-Simulation-Forage-

📌 Overview

This repository documents my work from the Deloitte Australia Data Analysis Job Simulation hosted on Forage. Through this simulation, I gained hands-on experience in analyzing real-world business data, applying forensic thinking, and creating interactive dashboards to support data-driven decision-making.

The simulation consisted of two key tasks, where I worked with tools such as Tableau and Microsoft Excel to extract insights and present findings clearly.

🧩 Tasks Completed
🔹 Task 1: Telemetry Data Analysis & Visualization (Tableau)

In this task, I analyzed machine telemetry data for a client named Daikibo, a manufacturing company operating across multiple global locations.

🏭 Client Background

Daikibo operates 4 factories:

🔹Daikibo Factory Meiyo – Tokyo, Japan

🔹Daikibo Factory Seiko – Osaka, Japan

🔹Daikibo Berlin – Berlin, Germany

🔹Daikibo Shenzhen – Shenzhen, China

Each factory contains 9 types of machines, and every machine sends a telemetry message every 10 minutes. The dataset covers one month of data (May 2021) and was provided as a single JSON file after being unified by the client’s tech team using a data unification algorithm.

🎯 Business Questions

The client collected this telemetry data to answer the following:

🔹Which factory experienced the most machine breakdowns?

🔹Which machine types broke down most frequently at that location?

🛠️ Tools & Techniques Used

🔹Tableau (Data import, calculated fields, dashboards)

🔹JSON data handling

🔹Data visualization & analysis

📊 Steps Performed in Tableau

🔹Imported the unified telemetry JSON dataset into Tableau

🔹Created a calculated measure named "Unhealthy", assigning:

🔹Value = 10 for each unhealthy status

(Represents 10 minutes of potential downtime per event)

🔹Built a bar chart: "Down Time per Factory"

🔹Built another bar chart: "Down Time per Device Type"

Designed an interactive dashboard:

🔹Combined both charts into one dashboard

🔹Enabled the factory chart as a filter, so selecting a factory updates machine-level downtime

🔹Identified the factory with the highest downtime and captured a dashboard screenshot as final output

🔹 Task 2: Forensic Technology – Gender Pay Equality Analysis (Excel)

In this task, I worked from a forensic technology perspective to help Daikibo Industrials investigate internal complaints related to gender-based salary inequality across different job roles and factory locations.

🧾 Background

After receiving several internal complaints regarding gender pay inequality, Daikibo Industrials initiated an internal investigation. The forensic technology team developed an algorithm to quantify gender pay equality levels across job roles and locations. As part of the team, my responsibility was to complete the analysis and help the client draw clear conclusions from the data.

The processed data was provided in an Excel file named Equality Table.xlsx, containing the following columns:

Factory

Job Role

Equality Score (integer ranging from -100 to +100, where 0 represents ideal equality)

🎯 Objective

To classify job roles based on the severity of gender pay inequality by creating a new derived column.

🛠️ Steps Performed in Excel

Analyzed the provided equality scores across factories and job roles

Added a 4th column named Equality Class

Classified each record using logical conditions:

Fair: Equality Score between -10 and +10

Unfair: Equality Score less than -10 or greater than +10

Highly Discriminative: Equality Score less than -20 or greater than +20

Used Excel formulas to automate classification and ensure consistency

🧮 Excel Formula Used

To classify the equality scores objectively, I used a nested IF function with the ABS() function to evaluate the magnitude of the equality score regardless of sign:

=IF(ABS(C2)<=10,"Fair",IF(ABS(C2)<=20,"Unfair","Highly Discriminative"))

Explanation:

ABS(C2) converts negative and positive scores to their absolute value

<= 10 → Fair

<= 20 → Unfair

> 20 → Highly Discriminative

📌 Examples

10 → Fair

-9 → Unfair

-30 → Highly Discriminative

The final output enabled the forensic team to quickly identify high-risk job roles and locations, supporting further investigation and corrective action.

This task strengthened my ability to:

Apply forensic thinking to real HR datasets

Use Excel for data classification and rule-based analysis

Translate numerical scores into clear, business-actionable insights

🧠 Key Learnings

Practical exposure to real-world business data analysis

Hands-on experience with Tableau dashboards and filters

Understanding of machine telemetry data and downtime analysis

Improved analytical thinking and forensic problem-solving

Translating technical findings into business-relevant insights

🧰 Skills Demonstrated

Data Analysis

Data Visualization (Tableau)

Dashboard Design

Excel-based Analysis

Business Insight Generation

Forensic Technology Concepts

📂 Repository Contents

Tableau dashboards (screenshots / files if applicable)

Supporting documentation

README explaining the project and approach

🔖 Acknowledgment

This project was completed as part of the Deloitte Australia Data Analysis Job Simulation on Forage, which provided an excellent opportunity to simulate real Deloitte-style client work and strengthen practical data analytics skills.
