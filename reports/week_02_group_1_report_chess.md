# Chess Report

---

## 1. Dataset Overview

| Item Description |                                                                                      |
|-------------------|--------------------------------------------------------------------------------------|
| Dataset name | Chess Game Dataset (Lichess)                                                         |
| Number of rows | 20058                                                                                |
| Number of columns | 16                                                                                   |
| Format file (.csv, .txt, etc) | .csv                                                                                 |
| Authors of the dataset | [Mitchell Jolly](https://mitchelljolly.com/)                                         |
| Source (name) | [Kaggle](https://www.kaggle.com/)                                                    |
| Source (link) | [Chess Game Dataset (Lichess)](https://www.kaggle.com/datasets/datasnaek/chess/data) |

**Short description (what is it about?)**

20,000+ Lichess Games, including moves, victor, rating, opening details and more

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
| Least frequent value             | –        | False | draw           | –      | –              | –        | -        | -     | -           | -                    |
| Least frequent value (frequency) | 1        | 3903  | 906            | 1      | 1              | 1        | 1        | 1     | 1           | 1                    |

**Note:** It is not possible to determine one least frequent value in many cases since there are often multiple instances of values occuring once.



---

## 4. Missing Values and Duplicates

| Column name    | Missing count | % Missing |
| -------------- | ------------- | --------- |
| id             | 0             | 0.00%     |
| rated          | 0             | 0.00%     |
| created_at     | 0             | 0.00%     |
| last_move_at   | 0             | 0.00%     |
| turns          | 0             | 0.00%     |
| victory_status | 0             | 0.00%     |
| winner         | 0             | 0.00%     |
| increment_code | 0             | 0.00%     |
| white_id       | 0             | 0.00%     |
| white_rating   | 0             | 0.00%     |
| black_id       | 0             | 0.00%     |
| black_rating   | 0             | 0.00%     |
| moves          | 0             | 0.00%     |
| opening_eco    | 0             | 0.00%     |
| opening_name   | 0             | 0.00%     |
| opening_ply    | 0             | 0.00%     |


**Total missing values:** 0
**Percentage of dataset affected:** 0%

**Duplicated rows found:** We found 429 identical tupels. However due to the quality of the dataset (e.g. rating in all caps and small caps) we suspect that there are more duplicated games that the exact duplicated rows.
Analysig the number of ids that occur more than once we found the following distribution of duplicated games:

| Occurrences per ID | Number of IDs |
| -----------------: | ------------: |
|                  5 |             1 |
|                  4 |            25 |
|                  3 |            79 |
|                  2 |           708 |
|                  1 |        18 300 |

This means that out of 20058 games only 19113 games are unique entries. Calculated adding the Number of IDs assuming that one game of the duplicated ID is valid.

**Percentage of rows in dataset affected:** 4.71%

---

## 5. Data Consistency

| Item | Description                                                                                                                                                                                                                                                                                                                      |
|------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Does the dataset contain unnecessary columns? Which? | Every opening has a fixed ammount of book moves. It is unnecessary to list them repeatedly.                                                                                                                                                                                                                                      |
| Do the data types correspond to the columns? | Yes. They match.                                                                                                                                                                                                                                                                                                                 |
| Is the labeling of the columns appropriate? | Yes. Precise. No further domain knowledge needed.                                                                                                                                                                                                                                                                                |
| Are there mixed values in a column (e.g., numbers and characters)? | Yes. The game id is a mix of numbers and characters.                                                                                                                                                                                                                                                                             |
| Are string columns clean? | yes. There are no issues with e.g. special characters.                                                                                                                                                                                                                                                                           |
| Does the dataset look machine generated? | Data from individual games look like authentic game generated data; However many games are noted multiple times, the data set seems to have been at least edited. Since there are two different types of TRUE/FALSE / True/False and different date formats we assume that the data has been stitched together from two sources. |
| Other | –                                                                                                                                                                                                                                                                                                                                |

---

## 6. Overall Assessment

- Is it worth it to further analyze the dataset? YES :)
- What possible analyses can be performed?
  - Analyze the impact of the opening on winning rate
  - Analyze the impact of rating and rating difference to the opponent
  - Analyze the advantage of playing white (starting the game)
  - Analyze the difference between rated and not rated games
  - Impact of the time format / increment code (possible correlation of time format and number of moves)
  - Identification of strange game developments (e.g "rage quit" after mouse slip 1.e3)


---

## 7. Next Steps

- **Handling missing values? How?** No missing values in the dataset


- **Removing duplicates?** yes. Duplicated games should be removed

- **Cleaning the columns? Which?** 
  - Normalize Date format
  - Normalize Rated (True/False) column

- **Creating a subset of the dataframe?** Dataset is no too big and can be handled entirely in general. 
  - Subset with only one game of each player
  - Subset for each opening

## 8. Short Summary

Generally an interesting dataset that can be understood with little domain knowledge of chess. It offers many opportunities for interesting analysis. The dataset was surprisingly "unclean" with around 4% of the games being duplicates. Additionally date and rated was not formatted well.
