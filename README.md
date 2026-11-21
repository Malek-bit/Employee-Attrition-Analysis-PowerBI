# 👥 Employee Attrition Analysis (Power BI)

An interactive Power BI dashboard that explores **who leaves a company, why, and what HR can do about it**. It was built as a college project and looks at attrition through tenure, age, income, work-life factors, satisfaction levels and promotion history.

![Who Leaves & Why](images/01-who-leaves-and-why.png)

---

## 📌 Business Problem

Employee turnover is costly: it means recruiting and training expenses, lost knowledge and lower team morale. HR leaders want to know:

1. **What is the overall attrition rate?**
2. **Which employees are most likely to leave?** (age, tenure, income, job level, marital status)
3. **How do work conditions affect attrition?** (overtime, distance from home, work-life balance, satisfaction)
4. **What should the company do to keep its people?**

---

## 📊 Dataset

- **File:** [`data/WA_Fn-UseC_-HR-Employee-Attrition.csv`](data/WA_Fn-UseC_-HR-Employee-Attrition.csv)
- **Size:** 1,470 employees × 35 columns, with no missing values
- **Target:** `Attrition` (Yes / No), which is **16.1%** Yes (237 employees)
- **Includes:** age, gender, marital status, education, department, job role and level, monthly income, overtime, distance from home, years at company, years in role, years since last promotion, years with current manager, and satisfaction scores (job, environment, relationship, work-life balance).

> Source: the **IBM HR Analytics Employee Attrition & Performance** sample dataset, publicly available on Kaggle. It is a fictional dataset created by IBM data scientists for analytics practice, so the findings illustrate analysis techniques and do not describe a real company.

---

## 🛠️ Tools & Skills

| Area | Details |
|---|---|
| **Tool** | Microsoft Power BI Desktop |
| **Data modeling** | Calculated columns that turn numeric fields into readable groups: `Age Generation`, `Age (bins)`, `Worked Year Group`, `EducationCategory`, `DistanceFromHome (bins)`, `YearsWithCurrManager (bins)`, `YearsSinceLastPromotion (bins)`, and satisfaction / work-life balance / job level categories |
| **DAX measures** | `Attrition Rate`, `Attritated Employees`, `Target Employee Count` |
| **Visuals** | Combo charts, 100% stacked columns, gauge, donut, pie, treemaps, matrix, clustered bar and column charts, multi-row cards, slicers |

---

## 🗂️ Dashboard Pages

### 1. Who Leaves & Why?
The main page. It shows the overall attrition rate on a gauge, and attrition by **tenure group**, **age** and **distance from home**. Slicers for overtime, age generation, education and gender let you filter the whole page.

![Who Leaves & Why](images/01-who-leaves-and-why.png)

### 2. Employees Life Work
Looks at the employee's working life: attrition by tenure and monthly income, by years with the current manager, by department and education, and the average years at the company, in the current role, with the current manager, and since the last promotion.

![Employees Life Work](images/02-employees-life-work.png)

### 3. Employees Satisfaction
Explores how satisfaction affects attrition: job satisfaction, environment satisfaction, relationship satisfaction, work-life balance and marital status.

![Employees Satisfaction](images/03-employees-satisfaction.png)

### 4. Some Major Solutions
Highlights the areas where action would have the biggest effect: overtime by department, work-life balance and relationship satisfaction, and job level against time since last promotion.

![Major Solutions](images/04-major-solutions.png)

---

## 🔍 Key Findings

| # | Finding | Evidence |
|---|---|---|
| 1 | **About 1 in 6 employees left.** | 237 of 1,470 employees, an attrition rate of **16.1%** |
| 2 | **Overtime is the strongest warning sign.** | Employees working overtime leave at about **30.5%**, versus about **10.4%** for those who don't. |
| 3 | **New employees are the most likely to leave.** | Employees in their first year leave at about **35%**, and attrition falls steadily with tenure (about 8% after 10+ years). |
| 4 | **Young employees leave the most.** | Employees aged 25 or under leave at about **36%**, versus about **9%** for ages 36–45. |
| 5 | **Low pay goes with higher attrition.** | Employees earning under 3,000 a month leave at about **29%**. Those who left earned about 4,800 on average, versus about 6,800 for those who stayed. |
| 6 | **Junior roles are the highest risk.** | Job level 1 attrition is about **26%**, versus about **5%** at level 4. |
| 7 | **Single employees leave far more often.** | About **25.5%** for single employees, versus about 12.5% for married and about 10% for divorced. |
| 8 | **A long commute pushes people out.** | Attrition is about **14%** within 5 km, rising to about **22%** beyond 20 km. |
| 9 | **Unhappy employees leave more.** | Job satisfaction 1 (lowest) leaves at about **23%**, versus about **11%** at level 4. Work-life balance 1 leaves at about **31%** (a small group of 80). |
| 10 | **Overtime hits some groups hardest.** | Single employees working overtime leave at about **50%**. |

---

## 💡 Recommendations

1. **Control overtime.** Review workloads, hire where overtime is routine, and monitor overtime hours as an early warning metric.
2. **Invest in the first year.** Strengthen onboarding, assign mentors, and run check-ins at 30, 90 and 180 days.
3. **Build career paths for junior and young employees.** Show clear promotion steps, since level 1 roles and early-career staff leave the most.
4. **Review pay at the lower end.** Check whether low-paid roles are competitive with the market.
5. **Offer flexibility for long commutes.** Remote or hybrid days could help employees who live far away.
6. **Track satisfaction and work-life balance.** Use short surveys and follow up quickly on low scores.

---

## 🚀 Future Improvements

- Add analysis of **job role**, **business travel** and **stock option level**, which are in the dataset but not yet in the dashboard.
- Add a written insights panel on each page, so the takeaway is visible without interpreting the charts.
- Build a prediction model to score each employee's attrition risk.

---

## ▶️ How to Open the Project

1. Install [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free, Windows).
2. Clone or download this repository.
3. Open `Employees_attrition_rate.pbix`.
4. If Power BI asks for the data source, point it to `data/WA_Fn-UseC_-HR-Employee-Attrition.csv`.

---

## 📁 Repository Structure

```
├── Employees_attrition_rate.pbix     # Power BI report
├── data/
│   └── WA_Fn-UseC_-HR-Employee-Attrition.csv
├── images/                           # Dashboard screenshots
│   ├── 01-who-leaves-and-why.png
│   ├── 02-employees-life-work.png
│   ├── 03-employees-satisfaction.png
│   └── 04-major-solutions.png
└── README.md
```

---

## 👤 Author

**Abdelmalek**
- GitHub: [@your-username](https://github.com/your-username)
- LinkedIn: _add your link_

⭐ If you found this project useful, feel free to star the repo!
