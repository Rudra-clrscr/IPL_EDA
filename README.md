# IPL EDA (2008--2017)

## 📌 Overview

This project performs **Exploratory Data Analysis (EDA)** on the Indian
Premier League (IPL) matches dataset for the period **2008--2017**.\
The analysis helps uncover insights such as: - Match outcomes\
- Teams' performance across seasons\
- Venues hosting the most matches\
- Distribution of wins by runs and wickets

## 📂 Dataset

The dataset used is **`matches.csv`**, which contains match-level
details such as: - `season` -- IPL season year\
- `city` -- City where the match was played\
- `venue` -- Stadium/ground details\
- `team1`, `team2` -- Competing teams\
- `winner` -- Match winner\
- `win_by_runs`, `win_by_wickets` -- Victory margins\
- `player_of_match` -- Best player of the match\
- `umpire1`, `umpire2`, `umpire3` -- Match umpires

👉 In preprocessing, `umpire3` was dropped (mostly missing), and
remaining null values were removed.

## ⚙️ Requirements

The notebook uses the following Python libraries:

``` bash
pandas
matplotlib
seaborn
```

Install them using:

``` bash
pip install pandas matplotlib seaborn
```

## 📊 Analysis Performed

1.  **Data Cleaning**
    -   Removed unnecessary column (`umpire3`)\
    -   Dropped rows with null values
2.  **Descriptive Statistics**
    -   Dataset info (`df.info()`)\
    -   Summary statistics (`df.describe()`)
3.  **Exploratory Visualizations**
    -   Matches won by each team (bar plot)\
    -   Matches hosted by each venue (bar plot)\
    -   Distribution of wins by runs (histogram)\
    -   Distribution of wins by wickets (histogram)\
    -   Toss decisions (bar plot)\
    -   Season-wise match count (bar plot)

## ▶️ Usage

1.  Clone/download this repo\

2.  Place the dataset (`matches.csv`) in the working directory\

3.  Open the notebook:

    ``` bash
    jupyter notebook IPL.ipynb
    ```

4.  Run all cells to reproduce the analysis

## 📈 Example Insights

-   Certain teams consistently dominate in number of wins\
-   Some venues host significantly more matches than others\
-   Wins by runs are skewed, while wins by wickets are more evenly
    distributed
