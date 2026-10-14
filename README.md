# 📊 HR & Talent Insights — Employee Performance and Salary Analysis

### People Analytics Consultant | Nexus Corp Case Study

## 📌 Project Overview

This project analyzes employee salary, department, years of experience, and performance scores for Nexus Corp.

The objective is to provide a descriptive overview of compensation patterns, identify high-performing employees, compare departmental performance, and examine the relationship between employee experience and salary.

Using Python and Pandas, this project transforms employee records into meaningful summaries and visualizations that can support preliminary HR and talent management discussions.

## 🎯 Project Objectives

- Calculate the company-wide average monthly salary.
- Compare average monthly salaries across departments.
- Identify employees with high performance scores.
- Calculate the number of high performers.
- Examine the relationship between years of experience and monthly salary.
- Compare average performance scores across departments.
- Present findings and recommendations based on the available data.

## 🗂️ Project Structure

```text
hr-talent-insights-analysis/
│
├── README.md
├── HR_Talent_Insights.ipynb
├── employee_performance_dataset.csv
└── hr_talent_insights_report.pdf
```

## 📁 Dataset Description

The dataset contains **20 employee records** and five original fields.

| Column | Description |
|---|---|
| `Employee_ID` | Unique employee identifier |
| `Department` | Department: HR, IT, Finance, or Marketing |
| `Years_of_Experience` | Employee experience in years |
| `Monthly_Salary` | Employee monthly salary |
| `Performance_Score` | Employee performance score from 1 to 10 |

A derived `High_Performer` column is created during the analysis.

### High-Performer Definition

An employee is classified as a high performer when their performance score is at least 7.

```python
df["High_Performer"] = df["Performance_Score"] >= 7
```

## 🛠️ Technologies Used

- **Python** — Programming language
- **Pandas** — Data manipulation and statistical calculations
- **Matplotlib** — Data visualization
- **Jupyter Notebook** — Interactive analysis
- **Google Colab** — Cloud-based notebook execution

## ⚙️ Analysis Workflow

### 1. Salary Benchmarking

Calculate the company-wide average monthly salary to establish a baseline for departmental comparisons.

### 2. Departmental Salary Comparison

Group employee records by department and compare employee counts and average monthly salaries.

### 3. High-Performer Identification

Filter employees with performance scores of 7 or above and review their department, experience, salary, and performance score.

### 4. High-Performer Headcount

Calculate the total number and percentage of employees classified as high performers, including a department-wise breakdown.

### 5. Experience vs. Salary

Use a scatter plot and Pearson correlation to examine the relationship between years of experience and monthly salary.

### 6. Departmental Performance Review

Calculate and compare average performance scores across HR, IT, Finance, and Marketing.

## 📈 Key Findings

The following results are taken from the accompanying PDF report.

### Company-Wide Salary Benchmark

| Metric | Result |
|---|---:|
| Employees analyzed | 20 |
| Average monthly salary | $55,159.65 |

### Average Monthly Salary by Department

| Department | Employees | Average Monthly Salary |
|---|---:|---:|
| Marketing | 6 | $65,270.33 |
| IT | 4 | $55,305.50 |
| HR | 5 | $52,361.40 |
| Finance | 5 | $45,708.40 |

**Key insight:** Marketing has the highest average monthly salary, while Finance has the lowest average monthly salary in this sample.

### High-Performer Analysis

The report defines employees with performance scores of 7 or above as high performers.

- **High performers:** 8 employees
- **Share of employees:** 40%
- **Marketing:** 3 high performers
- **Finance:** 2 high performers
- **HR:** 2 high performers
- **IT:** 1 high performer

The two highest performance scores are 10, achieved by employees `2010` and `2013`.

### Experience vs. Salary

- **Pearson correlation coefficient:** -0.277
- **Interpretation:** The report identifies a weak negative relationship between experience and monthly salary in this sample.

This result does not establish that experience reduces salary. The dataset contains only 20 employees and lacks additional compensation factors such as job role, grade, and location.

### Average Performance Score by Department

| Department | Average Performance Score |
|---|---:|
| Marketing | 5.83 |
| Finance | 5.80 |
| IT | 4.75 |
| HR | 4.20 |

**Key insight:** Marketing has the highest average performance score, closely followed by Finance. HR has the lowest average score in the supplied dataset.

## 💡 HR Insights and Recommendations

1. **Review salary differences:** Investigate departmental salary differences alongside job roles, seniority, responsibilities, and experience.
2. **Recognize high performers:** Use the analysis as a starting point for reviewing employee achievements and development opportunities.
3. **Investigate Finance compensation:** Finance has the lowest average salary despite a relatively high average performance score, warranting further contextual review.
4. **Support performance development:** Examine training needs and other organizational factors that may influence departmental performance.
5. **Collect additional HR data:** Include job grades, tenure, location, education, and role-level information for more meaningful compensation analysis.
6. **Avoid unsupported conclusions:** Use this small sample for exploratory analysis rather than definitive pay-equity or employee evaluation decisions.

## 📊 Visualizations

The accompanying report includes:

- Average monthly salary by department.
- Comparison of high-performing employees.
- Experience versus monthly salary scatter plot.
- Average performance score by department.

These visualizations help communicate compensation and performance patterns across the organization.

## 🚀 How to Run the Project

### Option 1: Google Colab

1. Open [Google Colab](https://colab.research.google.com/).
2. Upload `HR_Talent_Insights.ipynb`.
3. Upload `employee_performance_dataset.csv` when required.
4. Run the notebook cells sequentially.
5. Review the output tables, charts, and findings.

### Option 2: Run Locally

**Step 1 — Clone the repository**

```bash
git clone https://github.com/YOUR_USERNAME/hr-talent-insights-analysis.git
```

**Step 2 — Navigate to the project folder**

```bash
cd hr-talent-insights-analysis
```

**Step 3 — Install the required libraries**

```bash
pip install pandas matplotlib jupyter
```

**Step 4 — Launch Jupyter Notebook**

```bash
jupyter notebook
```

Open `HR_Talent_Insights.ipynb` and execute the cells.

**Note:** Ensure the notebook loads `employee_performance_dataset.csv` from the project directory. Update any Google Colab-specific upload code or file paths if necessary.

## 📄 Project Report

The `hr_talent_insights_report.pdf` file contains the detailed case study, including:

- Introduction and problem statement.
- Project objectives and dataset description.
- Salary benchmarking.
- Departmental salary comparison.
- High-performer identification.
- Headcount analysis.
- Experience versus salary analysis.
- Departmental performance review.
- Key findings and conclusion.

## ⚠️ Limitations

- The dataset contains only 20 employees.
- The analysis is descriptive and may not represent the wider organization.
- Salary comparisons do not account for role, seniority, location, or other compensation factors.
- Correlation does not establish causation.
- The results are not a complete pay-equity assessment or a substitute for a structured HR review.

## 🏁 Conclusion

The analysis identifies Marketing as the department with both the highest average monthly salary and the highest average performance score in the supplied sample. Finance has the lowest average salary but a relatively high average performance score.

Eight of the 20 employees meet the defined high-performer threshold. The weak negative experience–salary correlation highlights the need to consider job role, seniority, and other compensation factors before drawing conclusions.

The findings provide a starting point for further HR analysis, talent recognition, and compensation review using a larger and more detailed dataset.

## 👨‍💻 Author

**Abhinandan Babu Munnoli**

Aspiring AI & Machine Learning Engineer | Python Developer | Final-Year Computer Science Engineering Student

- **GitHub:** [Abhi-munnoli](https://github.com/Abhi-munnoli)
- **LinkedIn:** [Connect with me](https://www.linkedin.com/in/abhinandan-munnoli-361a932bb/)

---

⭐ If you find this project useful, consider giving the repository a star.

*Developed as an educational HR and people analytics case study.*
