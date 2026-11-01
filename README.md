# 📊 Students Performance – Exploratory Data Analysis

## 📌 Project Overview

This project focuses on performing Exploratory Data Analysis (EDA) on the StudentsPerformance dataset using Python.

The objective is to understand student academic performance and explore how factors such as parental education, lunch type, and test preparation relate to examination scores.

The project includes data cleaning, descriptive statistics, feature engineering, outlier detection, and data visualization to identify meaningful patterns in the dataset.

---

## 📁 Project Structure

```text
Students-Performance-EDA/
│
├── EDA7.ipynb
├── StudentsPerformance.csv
├── Student_Performance_Cleaned.csv
└── README.md
```

---

## 📂 Dataset Description

The dataset contains information about students, their backgrounds, and their academic performance in three subjects.

| Column                        | Description                                  |
| ----------------------------- | -------------------------------------------- |
| `gender`                      | Gender of the student                        |
| `race/ethnicity`              | Ethnic group of the student                  |
| `parental level of education` | Highest educational qualification of parents |
| `lunch`                       | Type of lunch received by the student        |
| `test preparation course`     | Test preparation course completion status    |
| `math score`                  | Mathematics examination score                |
| `reading score`               | Reading examination score                    |
| `writing score`               | Writing examination score                    |

### Feature Engineering

Two additional features were created:

* **Total Marks:** Sum of mathematics, reading, and writing scores (out of 300).
* **Percentage:** Overall percentage calculated from total marks.

Formula:

`Percentage = (Total Marks / 300) × 100`

---

## ⚙️ Analysis Workflow

### 1. Data Loading and Inspection

* Imported the dataset using Pandas.
* Examined the first few records and dataset dimensions.
* Checked column names, data types, missing values, and duplicates.

### 2. Data Cleaning

* Removed unnecessary leading and trailing spaces.
* Converted categorical values into lowercase.
* Checked for missing and duplicate records.

### 3. Descriptive Statistical Analysis

Calculated the following statistical measures for each subject:

* Mean
* Median
* Standard Deviation
* First Quartile (Q1)
* Second Quartile (Q2)
* Third Quartile (Q3)

### 4. Feature Engineering

* Created a `total marks` column.
* Calculated the overall `percentage` for each student.

### 5. Outlier Detection

* Applied the Interquartile Range (IQR) method.
* Used the 1.5 × IQR rule to identify potential outliers.
* Analysed outliers in mathematics, reading, and writing scores.

### 6. Data Export

Exported the cleaned dataset as:

`Student_Performance_Cleaned.csv`

### 7. Data Visualization

Created visualizations to explore score distributions and relationships between different variables.

---

## 📊 Data Visualizations

### 1. Average Scores by Parental Education

**Chart Type:** Grouped Bar Chart

Compares the average mathematics, reading, and writing scores across different parental education levels.

**Purpose:**

* Understand the relationship between parental education and student performance.
* Compare average scores across educational backgrounds.

<br>

<img width="308" height="197" alt="Screenshot 2026-10-31 112657" src="https://github.com/user-attachments/assets/02f40d60-34e8-40c4-ae06-3cc76965fe5d" />

<br><br><br>

---

### 2. Average Scores by Lunch Type

**Chart Type:** Grouped Bar Chart

Compares the average scores of students receiving standard lunch and free/reduced lunch.

**Purpose:**

* Identify differences in academic performance between lunch groups.
* Explore the possible relationship between socio-economic background and examination scores.

<br>

<img width="245" height="196" alt="Screenshot 2026-10-31 112827" src="https://github.com/user-attachments/assets/27c31d0a-d689-4472-9593-48606bfed27c" />

<br><br><br>

---

### 3. Mathematics Score Distribution by Test Preparation

**Chart Type:** Box Plot

Visualizes the distribution of mathematics scores based on whether students completed the test preparation course.

**Purpose:**

* Compare score distributions between the two groups.
* Examine median scores and variations.
* Identify potential outliers.

<br>

<img width="176" height="143" alt="Screenshot 2026-10-31 113443" src="https://github.com/user-attachments/assets/b20a84c6-a232-4948-b239-5c1178b697d9" />


<br><br><br>

---

### 4. Correlation Between Subject Scores

**Chart Type:** Correlation Heatmap

Displays the Pearson correlation coefficients between mathematics, reading, and writing scores.

**Purpose:**

* Identify the strength of relationships between subjects.
* Understand how performance in one subject relates to another.
* Compare correlations across all three subjects.

<br>

<img width="225" height="173" alt="Screenshot 2026-10-31 190135" src="https://github.com/user-attachments/assets/71d4e705-f318-43fb-85d7-cd00a935a4a6" />


<br><br><br>

---

## 🛠️ Technologies Used

| Technology       | Purpose                          |
| ---------------- | -------------------------------- |
| Python           | Programming and data analysis    |
| Pandas           | Data manipulation and cleaning   |
| NumPy            | Numerical operations             |
| Matplotlib       | Data visualization               |
| Seaborn          | Statistical visualization        |
| Jupyter Notebook | Interactive analysis environment |

---

## 📚 Key Concepts Applied

* Exploratory Data Analysis (EDA)
* Data Preprocessing and Cleaning
* Descriptive Statistics
* Feature Engineering
* GroupBy Operations and Aggregation
* Interquartile Range (IQR) Method
* Outlier Detection
* Data Visualization
* Correlation Analysis

---

## 🎯 Project Outcome

This project demonstrates the process of exploring and understanding a dataset using Python. It combines data cleaning, statistical analysis, feature engineering, and visualization to examine student academic performance.

The analysis helps identify patterns between student backgrounds, test preparation, and examination scores while providing practical experience with essential Python data analysis libraries.

---
