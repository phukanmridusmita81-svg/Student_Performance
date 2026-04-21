# Student Performance Analysis Dashboard
## Power BI Capstone Project

![Dashboard Preview](screenshots/page1_overview.png)

---

## Project Overview

This project is a **Power BI Capstone Dashboard** that analyses student academic performance across multiple dimensions including subjects, streams, gender, attendance, and study habits.

**Student Details:**
- **Name:** [Your Full Name]
- **Roll No:** [Your Roll Number]
- **Batch/Program:** [Your Batch Name]
- **Submission Date:** April 21, 2026

---

## Problem Statement

Educational institutions collect large amounts of student data every semester, but most of it sits unused in spreadsheets. Without a visual analytics tool, it is very difficult to:
- Identify which subjects have the highest failure rates
- Understand whether low attendance leads to poor marks
- Track gender-based differences in performance
- Spot at-risk students early enough for intervention

---

## Solution

A **4-page interactive Power BI Dashboard** built on a structured student dataset covering 15 students, 5 subjects each, across 3 streams — totalling 75 academic records.

### Dashboard Pages

| Page | Title | Key Visuals |
|------|-------|-------------|
| 1 | Overview KPI Summary | KPI cards, Stream bar chart, Gender Pass/Fail, Scatter plot |
| 2 | Subject Performance | Subject avg marks, Pass rate %, Risk coloring |
| 3 | Leaderboard & Grades | Top-5 students, Grade pie chart, Stream A+ count |
| 4 | Attendance & Study Hours | Attendance buckets, Study-hours line, City-wise marks |

---

## Screenshots

### Page 1 - Overview KPI Summary
![Page 1](screenshots/page1_overview.png)

### Page 2 - Subject Performance
![Page 2](screenshots/page2_subjects.png)

### Page 3 - Leaderboard & Grade Distribution
![Page 3](screenshots/page3_leaderboard.png)

### Page 4 - Attendance & Study Hours Impact
![Page 4](screenshots/page4_attendance.png)

---

## Tech Stack

| Technology | Purpose |
|------------|---------|
| Power BI Desktop | Primary dashboard and visualization tool |
| Python 3.x | Data generation and chart simulation |
| Pandas | Data manipulation |
| Matplotlib | Chart rendering |
| CSV / Excel | Data storage format |
| Git & GitHub | Version control |

---

## Project Structure

```
student_performance_project/
│
├── data/
│   └── student_data.csv          # Dataset (75 records)
│
├── dashboard/
│   └── generate_dashboard.py     # Python dashboard generator
│
├── screenshots/
│   ├── page1_overview.png        # KPI Overview Page
│   ├── page2_subjects.png        # Subject Analysis Page
│   ├── page3_leaderboard.png     # Leaderboard Page
│   └── page4_attendance.png      # Attendance Analysis Page
│
├── Project_Documentation.pdf     # Full project documentation (5 pages)
├── generate_pdf.py               # PDF generator script
└── README.md                     # This file
```

---

## Dataset Description

The dataset (`student_data.csv`) contains **75 rows** and **15 columns**:

| Column | Description |
|--------|-------------|
| Student_ID | Unique student identifier |
| Name | Student full name |
| Gender | Male / Female |
| Age | Age of student |
| City | Student's city |
| Stream | Science / Commerce / Arts |
| Subject | Subject name |
| Marks_Obtained | Marks scored (out of 100) |
| Max_Marks | Maximum marks (100) |
| Attendance_Percent | Attendance percentage |
| Study_Hours_Per_Day | Self-reported daily study hours |
| Grade | A+, A, B, C, D, F |
| Pass_Fail | Pass or Fail |
| Semester | Semester number |
| Year | Academic year |

---

## Key Insights

1. **Science stream** students show the most performance variation — from top scorers (96%) to at-risk students (38%)
2. **Attendance above 90%** correlates strongly with marks above 75
3. **Female students** in this dataset show a higher overall pass rate
4. **Mathematics and Chemistry** have the highest failure rates across all streams
5. **Study hours above 5/day** consistently produce A-grade outcomes

---

## Unique Features

- Color-coded risk indicators (Red = below 60, Orange = 60-74, Green = 75+)
- City-level geographic performance analysis
- Attendance-to-marks correlation study
- Medal-style leaderboard for top performers
- Multi-stream, multi-subject, multi-dimension analysis in one report

---

## Future Improvements

- Real-time database integration (SQL Server / MySQL)
- Machine learning model for predicting at-risk students
- Role-based access: separate views for parents, teachers, and admins
- Semester-over-semester trend analysis
- Power BI Service deployment with mobile optimization

---

## How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/student-performance-dashboard.git
   ```

2. Install Python dependencies:
   ```bash
   pip install pandas matplotlib seaborn reportlab openpyxl
   ```

3. Generate dashboard visuals:
   ```bash
   cd dashboard
   python generate_dashboard.py
   ```

4. Open `data/student_data.csv` in Power BI Desktop to rebuild the live dashboard.

---

## Submission

- **Project ZIP:** Submitted via Google Form
- **GitHub:** This repository
- **Documentation PDF:** `Project_Documentation.pdf`

---

*This project is original work submitted as part of the Power BI Capstone evaluation.*
