![vecteezy_magnifying-glass-and-documents-with-analytics-data-lying-on_5128487](https://github.com/user-attachments/assets/88d20fff-e575-4cbb-bad6-773d106aa7fe)


This repository contains a complete workflow for preparing and analyzing manufacturing quality data from PrecisionTech Manufacturing, a producer of precision metal components.
The project is divided into two phases:

**Data Preprocessing**

**Business Problem Analysis using Statistical Methods**

## Phase 1: Data Preprocessing

Performed essential preprocessing to make the datasets analysis-ready:

Handled missing values (mean/median/mode)

Fixed invalid entries & inconsistent labels

Converted data types (datetime, numeric, categorical)

Removed outliers using IQR & domain rules

Reshaped datasets using melt/merge operations

Engineered features such as DaysSinceCalibration, MeasurementDeviation, etc.

This ensures clean, reliable data for statistical tests.

## Phase 2: Statistical Analysis

Addressed multiple business questions using proper statistical techniques:

### **1. Length Spec Verification**

**Test:** One-sample z-test

Checked if the average Length_mm meets the 50 mm specification.

### **2. Defect Rates by Shift**

**Test:** Chi-square test

Compared Morning vs Night shift defect patterns.

### 3. Material Yield Comparison

**Test:** One-way ANOVA

Identified which material type yields the highest BatchYield%.

### **4. Operator Experience vs Defects**

**Test:** Correlation / Two-sample t-test

Analyzed whether experienced operators produce fewer defects.

### **5. Supplier Quality Impact**

**Test:** Pearson correlation / Linear regression

Checked if Supplier QualityScore relates to defect counts.

### **6. Machine Age & Diameter Variance**

**Test:** Levene’s test / ANOVA

Evaluated whether older machines produce greater diameter variability.

### **7. Calibration Drift**

**Test:** Linear regression

Studied how days since last calibration impact measurement deviation.

### **8. Yield Differences by Department**

**Test:** One-way ANOVA

Compared BatchYield% across Production, QA, and Maintenance departments.

## Tools & Libraries

**Python**

**Pandas**

**NumPy**

**SciPy / Statsmodels**

**Matplotlib / Seaborn**

**Jupyter Notebook**

## Key Outcomes

Built a complete data cleaning pipeline for manufacturing datasets.

Applied rigorous statistical tests to answer real business questions.

Produced insights useful for quality improvement, process control, and decision-making.
