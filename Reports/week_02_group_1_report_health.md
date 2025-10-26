# Basic EDA of Two Datasets – Report Structure for Week 2

---

## 1. Dataset Overview

| Item Description |   |
|-------------------|---|
| Dataset name | Sleep_health_and_lifestyle_dataset.csv  |
| Number of rows |  374 |
| Number of columns |  13 |
| Format file (.csv, .txt, etc) | csv  |
| Authors of the dataset | Kaggle contributor (Laksika Tharmalingam )  |
| Source (name) |  Kaggle |
| Source (link) |  https://www.kaggle.com/datasets/uom190346a/sleep-health-and-lifestyle-dataset |

**Short description (what is it about?)**  
Sleep health metrics and related lifestyle factors.

---

## 2. Structure of the Dataset

| Column name | Data type | Non-null count | Unique values | Example values |
|--------------|------------|----------------|----------------|----------------|
| Person ID | int | 374 | 374 | 1, 2, 3 |
| Gender | string | 374 | 2 | Male, Female |
| Age | int | 374 | 31 | 27, 28, 29 |
| Occupation | string | 374 | 11 | Software Engineer, Doctor, Sales Representative |
| Sleep Duration | float | 374 | 27 | 6.1, 6.2, 5.9 |
| Quality of Sleep | int | 374 | 6 | 6, 4, 7 |
| Physical Activity Level | int | 374 | 16 | 42, 60, 30 |
| Stress Level | int | 374 | 6 | 6, 8, 7 |
| BMI Category | string | 374 | 4 | Overweight, Normal, Obese |
| Blood Pressure | string | 374 | 25 | 126/83, 125/80, 140/90 |
| Heart Rate | int | 374 | 19 | 77, 75, 85 |
| Daily Steps | int | 374 | 20 | 4200, 10000, 3000 |
| Sleep Disorder | string | 374 | 3 | None, Sleep Apnea, Insomnia |

---

## 3. Descriptive Statistics

### Numeric Columns

|   | Person ID | Age | Sleep Duration | Quality of Sleep | Physical Activity Level | Stress Level | Heart Rate | Daily Steps |
|---|------------|-----|----------------|------------------|--------------------------|--------------|-------------|--------------|
| Count | 374.0 | 374.0 | 374.0 | 374.0 | 374.0 | 374.0 | 374.0 | 374.0 |
| Mean | 187.50 | 42.18 | 7.13 | 7.31 | 59.17 | 5.39 | 70.17 | 6816.84 |
| Standard deviation | 108.11 | 8.67 | 0.80 | 1.20 | 20.83 | 1.77 | 4.14 | 1617.92 |
| Min | 1.0 | 27.0 | 5.8 | 4.0 | 30.0 | 3.0 | 65.0 | 3000.0 |
| 25% | 94.25 | 35.25 | 6.4 | 6.0 | 45.0 | 4.0 | 68.0 | 5600.0 |
| 50% | 187.5 | 43.0 | 7.2 | 7.0 | 60.0 | 5.0 | 70.0 | 7000.0 |
| 75% | 280.75 | 50.0 | 7.8 | 8.0 | 75.0 | 7.0 | 72.0 | 8000.0 |
| Max | 374.0 | 59.0 | 8.5 | 9.0 | 90.0 | 8.0 | 86.0 | 10000.0 |

### Categorical / Object Columns

| Column | Count | Unique | Most frequent | Most frequent (freq) | Least frequent | Least frequent (freq) |
|---|---|---|---|---|---|---|
| Gender | 374 | 2 | Male | 189 | Female | 185 |
| Occupation | 374 | 11 | Nurse | 73 | Manager | 1 |
| BMI Category | 374 | 4 | Normal | 195 | Obese | 10 |
| Blood Pressure | 374 | 25 | 130/85 | 99 | 121/79 | 1 |
| Sleep Disorder | 374 | 3 | None | 219 | Insomnia | 77 |

---

## 4. Missing Values and Duplicates

| Column name | Missing count | % Missing |
|--------------|----------------|------------|
| Person ID | 0 | 0.0 |
| Gender | 0 | 0.0 |
| Age | 0 | 0.0 |
| Occupation | 0 | 0.0 |
| Sleep Duration | 0 | 0.0 |
| Quality of Sleep | 0 | 0.0 |
| Physical Activity Level | 0 | 0.0 |
| Stress Level | 0 | 0.0 |
| BMI Category | 0 | 0.0 |
| Blood Pressure | 0 | 0.0 |
| Heart Rate | 0 | 0.0 |
| Daily Steps | 0 | 0.0 |
| Sleep Disorder | 0 | 0.0 |

**Total missing values:** 0  
**Percentage of dataset affected:** 0.0%  

**Duplicated rows found:** 0  
**Percentage of rows in dataset affected:** 0.0%

---

## 5. Data Consistency

| Item | Description |
|------|--------------|
| Does the dataset contain unnecessary columns? Which? | Person ID (identifier, may not be analytically needed) |
| Do the data types correspond to the columns? | Yes, all data types are appropriate. |
| Is the labeling of the columns appropriate? | Yes, column names are descriptive and clear. |
| Are there mixed values in a column (e.g., numbers and characters)? | No, columns are consistent. |
| Are string columns clean? | Mostly clean, trimming or case standardization may help. |
| Does the dataset look machine generated? | Yes, Person ID column suggests synthetic generation and also the author confirmed that the dataset is synthetic and was created for illustrative purposes.|
| Other |  |

---

## 6. Overall Assessment

- Is it worth it to further analyze the dataset?  
  Yes, it’s clean, complete, and contains meaningful lifestyle and sleep health variables suitable for analysis.

- What possible analyses can be performed?  
  Correlation analysis, group comparisons (e.g., by gender or BMI), visualization of sleep and stress patterns, or predictive modeling of sleep disorders.

---

## 7. Next Steps

- Handling missing values? How?  
  No missing values because no imputation needed.

- Removing duplicates?  
  None found, no action required.

- Cleaning the columns? Which?  
  Minor cleaning can be helped like trim whitespace and standardize text case but not neccessary.

- Creating a subset of the dataframe?  
  

