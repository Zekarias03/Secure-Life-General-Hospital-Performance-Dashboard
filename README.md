# Secure-Life-General-Hospital-Performance-Dashboard
![](Introductory_Image.png)
## 1. Introduction
Hospitals record a large amount of information every day: who was admitted, where they were treated, how long they stayed, what the bill was and how it was paid. On its own, this information is hard to use. In this project, I analysed patient admission, billing and insurance records for Secure Life General Hospital using Microsoft Excel and built an interactive dashboard. The goal was to give hospital management one clear view of patient demand, departmental performance, payments and insurance coverage, so that they can spot problems early and make better decisions.
## 2. About the Dataset
The dataset contains 1,000 patient visits recorded between January 2024 and December 2025 (a few discharges fall in early January 2026). Each row is one visit, not one unique patient, so a patient can appear more than once. The original data has 11 columns:
• Patient information: Patient ID, Patient Name, Age, Gender
• Admission details: Admission Date, Discharge Date, Department
• Medical information: Diagnosis
• Billing and payment: Total Bill Amount, Insurance Coverage (%), Payment Status (Paid, Pending or Partially Paid)
To support the analysis, I added helper columns for length of stay, age group, admission year and outstanding amount. Age groups are Under 18, 18-35, 36-50, 51-65 and 66 & Above.
## 3. Problem Statement
The management of Secure Life General Hospital noticed changes in patient admissions, outstanding medical bills and insurance coverage across departments. However, the hospital had no consolidated report showing its operational and financial performance. Without one, it is difficult to see which departments are busiest, where the money is billed, how much is still unpaid and how insurance coverage differs across services.
My task as the data analyst was to turn the raw records into insights and build an interactive dashboard that answers these questions:
1. How many patient visits has the hospital recorded?
2. Which departments receive the most patients?
3. Which departments generate the highest total bills?
4. What is the average length of stay in each department?
5. What share of bills is paid, pending or partially paid?
6. How much has the hospital billed, and how much is outstanding?
7. How does insurance coverage vary across departments and diagnoses?
8. Which age groups account for the most visits?
9. How do admissions and billing change over time?
10. Which areas need management attention?
## 4. Tools Used
• Microsoft Excel: formulas, PivotTables, PivotCharts and slicers
• GitHub: project documentation
## 5. Dashboard Visualization
[Paste Dashboard_Image here]
The dashboard brings the main indicators into one screen: key figures (total visits, total bills, paid amount, average stay and average insurance coverage), patients by department, payment status, gender split, age groups and the admission trend over time. Slicers for department, payment status and year let users filter the whole dashboard without opening the raw records.
## 6. Key Insights and Findings
- 1. Patient visits. The hospital recorded 1,000 visits. Female patients accounted for 512 visits (51.2%) and male patients for 488 (48.8%), so the split is almost even.
- 2. Busiest departments. General received the most visits (252, or 25.2%), followed by Emergency (190, 19.0%), Orthopedics (159), Pediatrics (153) and Cardiology (152). Neurology received the fewest (94).
- 3. Highest bills. The hospital billed $8,053,143 in total. Orthopedics generated the most at about $2.55 million (31.7% of all billing), followed by Cardiology at $2.10 million (26.0%) and Neurology at $1.22 million (15.1%). General, which has the most visits, accounts for only 12.3% of billing. The reason is the cost per visit: the average bill is about $16,100 in Orthopedics, $13,800 in Cardiology and $12,900 in Neurology, compared with about $3,900 in General and $3,300 in Emergency.
- 4. Length of stay. The average stay is 4.8 days. Orthopedics has the longest stay (8.4 days), followed by Neurology (6.9) and Cardiology (6.5). Emergency has the shortest (2.0 days). In total, 101 visits lasted 10 days or more.
- 5. Payment status. 564 visits (56.4%) are fully paid, 257 (25.7%) are pending and 179 (17.9%) are partially paid. This means 43.6% of visits are not fully settled.
- 6. Billed and outstanding. Of the $8,053,143 billed, $4,568,527 (56.7%) belongs to fully paid visits. The remaining $3,484,616 (43.3%) belongs to pending visits ($2,082,786) and partially paid visits ($1,401,830). The data has no amount-paid column, so the part already received on partially paid bills cannot be separated. The true outstanding amount is therefore at most $3,484,616.
- 7. Insurance coverage. Average coverage is 74.9%. Across departments it is fairly even, from 73.9% in General to 76.3% in Cardiology. It varies more by diagnosis: Coronary Artery Disease (82.9%), Stroke (82.2%) and RSV (80.8%) have the highest coverage, while Asthma (61.5%), Arrhythmia (63.5%) and Epilepsy (67.9%) have the lowest. In addition, 44 visits had no insurance coverage at all, worth $345,195 in bills.
- 8. Age groups. Patients aged 51-65 made the most visits (235, 23.5%), followed by those aged 66 and above (232, 23.2%), 36-50 (210), 18-35 (170) and under 18 (153). Patients aged 51 and above account for 467 visits, or 46.7% of the total.
- 9. Trends over time. There were 508 visits in 2024 and 492 in 2025, and billing fell from about $4.13 million to $3.92 million. Admissions were steady in 2024 (34 to 51 a month) but more uneven in 2025. The busiest month was November 2025 with 57 visits and about $510,000 billed. The quietest months were June and August 2025 with 29 visits each, and June 2025 also had the lowest billing (about $191,000).
- 10. Areas needing attention. Orthopedics holds the largest unpaid balance (about $1.10 million, 31% of the total), followed by Cardiology ($0.90 million). General has the highest share of visits not fully paid (46.8%), and Pediatrics is close behind (46.4%). Orthopedics also has the longest stays, and a number of diagnoses have low or no insurance coverage.
## 7. Recommendations
1. Follow up unpaid bills, starting with Orthopedics and Cardiology. Together they hold more than half of the outstanding amount, so collection efforts there will recover the most money.
2. Improve payment follow-up in General and Pediatrics. Nearly half of their visits are not fully paid, which points to a weakness in billing or reminders, not just large bills.
3. Record payments in the data. Adding an amount-paid column would show exactly how much is outstanding on partially paid bills and make future reporting accurate.
4. Plan beds and staff by length of stay as well as visit numbers. Orthopedics, Neurology and Cardiology have long stays and high bills, so they use more resources per patient than their visit counts suggest.
5. Review insurance arrangements for low-coverage diagnoses. Asthma, Arrhythmia and Epilepsy have the lowest coverage, and the 44 visits with no coverage leave patients with large bills that are harder to collect.
6. Prepare for peak months. November 2025 had the highest admissions, so staffing and capacity should be reviewed before similar periods.
## 8. Conclusion
This project shows how Excel can turn raw hospital records into information that supports decisions. The main finding is that the busiest department is not the one that earns the most: General has the most visits but Orthopedics and Cardiology produce more than half of total billing because each visit costs much more and lasts longer. The analysis also shows that 43.3% of the amount billed has not been fully paid, which is the clearest area for management action. Overall, the project strengthened my skills in data cleaning, PivotTables, dashboard design and communicating findings in a simple way.
