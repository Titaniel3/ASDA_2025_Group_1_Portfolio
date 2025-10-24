# Chess Report

---

## 1. Dataset Overview

| Item Description |      |
|-------------------|------|
| Dataset name |      |
| Number of rows |      |
| Number of columns |      |
| Format file (.csv, .txt, etc) | .csv |
| Authors of the dataset |      |
| Source (name) |      |
| Source (link) |      |

**Short description (what is it about?)**

The dataset contains information of 20.000 chess matches. It lists general information about the match and provides a step-by-step documentation about the moves that were played.

---

## 2. Structure of the Dataset

| Column name    | Data type | Non-null count | Unique values | Example values                                                                                                          |
|----------------|-----------|----------------|---------------|-------------------------------------------------------------------------------------------------------------------------|
| id             | object    | 20058          | 19113         | kWKvrqYL                                                                                                                |
| rated          | bool      | 20058          | 2             | TRUE                                                                                                                    |
| created_at     | float64   | 20058          | 13151         | 1.49777E+12                                                                                                             |
| last_move_at   | float64   | 20058          | 13186         | 1.48376E+12                                                                                                             |
| turns          | int64     | 20058          | 211           | 105                                                                                                                     |
| victory_status | object    | 20058          | 4             | draw                                                                                                                    |
| winner         | object    | 20058          | 3             | white                                                                                                                   |
| increment_code | object    | 20058          | 400           | 15+5                                                                                                                    |
| white_id       | object    | 20058          | 9438          | ravoshm                                                                                                                 |
| white_rating   | object    | 20058          | 1516          | 1286                                                                                                                    |
| black_id       | int64     | 20058          | 9331          | crixin                                                                                                                  |
| black_rating   | object    | 20058          | 1521          | 1422                                                                                                                    |
| moves          | int64     | 20058          | 18920         | e4 e5 Nf3 Nc6 Bc4 Nf6 Ng5 d5 exd5 Nxd5 d3 f6 Ne4 Nd4 Qh5+ g6 Nxf6+ Qxf6 Qg4 Nxc2+ Ke2 Bxg4+ f3 Nxa1 fxg4 Nf4+ Ke1 Nxd3+ |
| opening_eco    | object    | 20058          | 365           | B06                                                                                                                     |
| opening_name   | object    | 20058          | 1477          | King's Indian Defense: Normal Variation                                                                                 |  King's Knight Variation           |
| opening_ply    | int64     | 20058          | 23            | 9                                                                                                                       |

**Note:** The lower unique number of ids already indicates that the data set is not entirely cleaned of dublicates yet. There are games that are documented multiple times using the same id (e.g. id 3IGubBMZ).


---

## 3. Descriptive Statistics

### Numeric Columns

|                    | created_at           | last_move_at         | turns | white_rating | black_rating | opening_ply |
|--------------------|----------------------|----------------------|-------|--------------|--------------|-------------|
| Count              | 20058                | 20058                | 20058 | 20058        | 20058        | 20058       |
| Mean               | 1,483,617,000,000.00 | 1,483,618,000,000.00 | 60.47 | 1,596.63     | 1,588.83     | 4.82        |
| Standard deviation | 28,501,510,000.00    | 28,501,400,000.00    | 33.57 | 291.25       | 291.04       | 2.80        |
| Min                | 1,376,772,000,000.00 | 1,376,772,000,000.00 | 1     | 784          | 789          | 1           |
| 25%                | 1,477,548,000,000.00 | 1,477,548,000,000.00 | 37    | 1,398        | 1,391        | 3           |
| 50%                | 1,496,010,000,000.00 | 1,496,010,000,000.00 | 55    | 1,567        | 1,562        | 4           |
| 75%                | 1,503,170,000,000.00 | 1,503,170,000,000.00 | 79    | 1,793        | 1,784        | 6           |
| Max                | 1,504,493,000,000.00 | 1,504,494,000,000.00 | 349   | 2,700        | 2,723        | 28          |

**Note:** The following columns do not appear in this chart due to the values not being numeric: rated, victory_status, winner, increment_code, white_id, black_id, moves, opening_eco, opening_name. They will be described further in the following object columns table.


### Categorical / Object Columns

|                                  | id       | rated | victory_status | winner | increment_code | white_id | black_id | moves | opening_eco | opening_name         |
|----------------------------------|----------|-------|----------------|--------|----------------|----------|----------|-------|-------------|----------------------|
| Count                            | 20058    | 20058 | 20058          | 20058  | 20058          | 20058    | 20058    | 20058 | 20058       | 20058                |
| Number of unique values          | 19113    | 2     | 4              | 3      | 400            | 9438     | 9331     | 18920 | 365         | 1477                 |
| Most frequent value              | XRuQPSzH | True  | resign         | white  | 10+0           | taranga  | taranga  | e4 e5 | A00         | Van't Kruijs Opening |
| Most frequent value (frequency)  | 5        | 16155 | 11147          | 10001  | 7721           | 72       | 82       | 27    | 1007        | 368                  |
| Least frequent value             |          |       |                |        |                |          |          |       |             |                      |
| Least frequent value (frequency) |          |       |                |        |                |          |          |       |             |                      |

**Note:** It is not possible to determine one least frequent value in many cases since there are often multiple instances of values occuring once.



---

## 4. Missing Values and Duplicates

| Column name | Missing count | % Missing |
|--------------|----------------|------------|
|   |   |   |
|   |   |   |
|   |   |   |

**Total missing values:**  
**Percentage of dataset affected:**  

**Duplicated rows found:**  
**Percentage of rows in dataset affected:**

---

## 5. Data Consistency

| Item | Description                                                                                                                                                      |
|------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Does the dataset contain unnecessary columns? Which? |                                                                                                                                                                  |
| Do the data types correspond to the columns? |                                                                                                                                                                  |
| Is the labeling of the columns appropriate? |                                                                                                                                                                  |
| Are there mixed values in a column (e.g., numbers and characters)? |                                                                                                                                                                  |
| Are string columns clean? |                                                                                                                                                                  |
| Does the dataset look machine generated? | Data from individual games look like authentic game generated data; However many ames are noted multiple times, the data set seems to have been at least edited. |
| Other |                                                                                                                                                                  |

---

## 6. Overall Assessment

- Is it worth it to further analyze the dataset?  
- What possible analyses can be performed?

---

## 7. Next Steps

- Handling missing values? How?  
- Removing duplicates?  
- Cleaning the columns? Which?  
- Creating a subset of the dataframe?  
