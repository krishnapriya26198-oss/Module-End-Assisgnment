# Healthcare Data Analysis Using Microsoft Excel

## Project Overview

This project focuses on cleaning, transforming, analyzing, and visualizing healthcare data using Microsoft Excel. The objective is to explore patient health indicators, demographic information, and healthcare charges to identify patterns and relationships within the dataset.

The project uses three datasets: Customer Names, Medical Examinations, and Hospitalization Details. These datasets are prepared and combined using Customer ID to create a consolidated healthcare dataset for analysis.

## Project Objectives

* Identify and handle missing data.
* Standardize inconsistent values and transform raw data.
* Categorize patients according to BMI and HbA1C levels.
* Calculate patient age using date information.
* Combine multiple datasets using VLOOKUP.
* Analyze relationships between patient health indicators and healthcare charges.
* Create charts using PivotTables and PivotCharts.
* Develop an interactive dashboard with slicers.

## Tools and Technologies

* Microsoft Excel
* VLOOKUP
* IF and DATE functions
* PivotTables and PivotCharts
* Data cleaning and transformation
* Data visualization
* Dashboard development

---

## 1. Data Cleaning — 5 Marks

### 1.1 Missing Value Identification

Checked the number of missing values marked with `?` in each column of the Medical Examinations and Hospitalization Details tables.

### 1.2 Missing Month and Year Values

* Replaced missing month values with `Sep`.
* Replaced missing year values with the average year rounded to the nearest integer.

### 1.3 Most Frequent Values

Identified the most frequently occurring values in the following columns and used them to fill missing entries:

* `smoker`: No
* `Hospital tier`: Tier 2
* `City tier`: Tier 2

### 1.4 Missing State ID Values

Replaced missing State ID values with `Unknown`.

---

## 2. Data Transformation — 8 Marks

### 2.1 Customer Name Transformation

Split the `names` column in the Customer Names table into three meaningful columns:

* Title
* First Name
* Last Name

### 2.2 Major Surgery Data Conversion

Converted `NumberOfMajorSurgeries` into numerical data by replacing the text value `No major surgery` with `0`.

### 2.3 Data Consistency

Checked the `Heart Issues` and `smoker` columns for inconsistent capitalization and standardized categorical values.

### 2.4 BMI Classification

Created a new column called `Weight Status` based on BMI values.

| BMI Range      | Weight Status |
| -------------- | ------------- |
| Below 18.5     | Underweight   |
| 18.5–24.9      | Normal Weight |
| 25.0–29.9      | Overweight    |
| 30.0 and above | Obesity       |

### 2.5 HbA1C Classification

Created a new column called `Diabetes Status` based on HbA1C values.

| HbA1C Range   | Diabetes Status |
| ------------- | --------------- |
| Below 5.7     | Normal          |
| 5.7–6.4       | Prediabetes     |
| 6.5 and above | Diabetes        |

### 2.6 Date of Birth Creation

Combined the `year`, `month`, and `date` columns in the Hospitalization Details table into one column named `Date of Birth`.

The date format was set to `DD-MMM-YYYY`.

### 2.7 Age Calculation

Calculated customer age using June 8, 2023, as the dataset collection date.

### 2.8 Currency Formatting

Formatted the `charges` column as currency in dollars ($).

---

## 3. Data Exploration, Analysis and Visualization — 12 Marks

### 3.1 Dataset Consolidation

Created a new worksheet named `Healthcare` by combining the three datasets using Customer ID as the common identifier and VLOOKUP.

The consolidated dataset retains the following columns:

* Customer ID
* First Name
* BMI
* HBA1C
* Heart Issues
* Any Transplants
* Cancer history
* NumberOfMajorSurgeries
* smoker
* Weight Status
* Diabetes Status
* Date of Birth
* charges
* Hospital tier
* City tier
* State ID
* Age

### 3.2 Pie/Donut Chart Analysis

**Analysis 1: Cancer History Among Smokers and Non-Smokers**

Examined the distribution of cancer history among smokers and non-smokers using a pie chart.

**Analysis 2: Transplant History, Major Surgeries and HbA1C**

The assignment requires comparing the total number of major surgeries and average HbA1C between patients with and without a history of transplants. This analysis should be presented using an appropriate chart or charts.

### 3.3 Column/Bar Chart Analysis

**Analysis 3: Healthcare Charges by Weight Status and Diabetes Status**

Compared healthcare charges across different weight-status and diabetes-status categories using a column chart.

**Analysis 4: Average Charges by Hospital Tier and State**

The assignment requires comparing average healthcare charges for each hospital tier across different states. An appropriate column or bar chart should be used to present this comparison.

### 3.4 Line/Scatter Plot Analysis

**Analysis 5: Age, BMI and HbA1C**

The assignment requires exploring relationships between age and both BMI and HbA1C using an appropriate line or scatter plot.

**Analysis 6: Age and Healthcare Charges**

Created a line chart to explore the relationship between patient age and healthcare charges.

These visualizations support the exploration of patterns in the healthcare dataset. Correlation or causation should not be assumed from a chart alone.

---

## 4. Interactive Dashboard

The objective is to consolidate the key visualizations into a single Excel dashboard with clear titles, readable labels, and an organized layout.

### Planned Dashboard Components

* Pie chart showing cancer history among smokers and non-smokers.
* Chart comparing total major surgeries and average HbA1C by transplant history.
* Column chart comparing healthcare charges by Weight Status and Diabetes Status.
* Chart comparing average charges by hospital tier and state.
* Visualization exploring age in relation to BMI and HbA1C.
* Line or scatter chart exploring age and healthcare charges.

### Interactive Slicers

Two slicers are required:

1. **Weight Status** — to filter by Underweight, Normal Weight, Overweight, and Obesity.
2. **Diabetes Status** — to filter by Normal, Prediabetes, and Diabetes.

The slicers should be connected to the relevant PivotTables so that they filter all applicable visualizations together. Their connections must be tested to ensure that the dashboard behaves as intended.

**Dashboard status:** The pie, column, and line charts have been created. The consolidated dashboard, remaining required visualizations, and slicer connections still need to be finalized and verified.

---

## 5. Key Skills Demonstrated

* Data cleaning and missing-value handling
* Data standardization and transformation
* Excel formulas and conditional logic
* VLOOKUP and dataset consolidation
* PivotTable and PivotChart creation
* Exploratory data analysis
* Healthcare data visualization
* Interactive dashboard development

---

## 6. Conclusion

This project demonstrates how Microsoft Excel can be used to prepare healthcare data, create meaningful patient categories, combine multiple datasets, and explore healthcare charges through visual analysis.

The project provides a foundation for investigating how factors such as age, BMI, HbA1C, smoking status, cancer history, transplant history, and hospital tier relate to healthcare costs and patient characteristics.

The completed and remaining visualizations will support a clearer understanding of the dataset and help communicate findings in a structured and accessible format.

---

## 7. Project Completion Checklist

### Data Cleaning

* [x] Check missing values in both tables
* [x] Fill missing month and year values
* [x] Fill missing smoker and tier values using the most frequent categories
* [x] Handle missing State ID values

### Data Transformation

* [x] Split names into Title, First Name, and Last Name
* [x] Convert major surgery descriptions into numerical values
* [x] Standardize inconsistent categorical values
* [x] Create Weight Status
* [x] Create Diabetes Status
* [x] Create and format Date of Birth
* [x] Calculate Age
* [x] Format charges as currency

### Data Exploration and Visualization

* [x] Combine datasets into the Healthcare worksheet
* [x] Create a pie chart
* [x] Create a column chart
* [x] Create a line chart
* [ ] Complete and verify all six required analyses and their visualizations

### Dashboard

* [ ] Consolidate all required charts into the dashboard
* [ ] Add the Weight Status slicer
* [ ] Add the Diabetes Status slicer
* [ ] Connect slicers to all applicable PivotTables
* [ ] Test interactive filtering across the visualizations

---

## Author

Healthcare Data Analysis Project

**Tools Used:** Microsoft Excel
