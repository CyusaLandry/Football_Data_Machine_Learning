# Football Data Machine Learning
Names: Cyusa Niyibaho Landry
Id: 25539
## Project Objective: Can We Model The Likelihood of a Match ending in a Win,Loss or Draw By Using Team Stats and Bookmaker Odds
### DataSet Title: English Football Data
### DataSet Link: https://example.com](https://www.football-data.co.uk/englandm.php
### Dataset Description
####   - DataSet Description: 27 CSV Files Containing Data of all matches from the top 3 divisions in england from **2016/17 to 2024/25** 
####   - Number of Rows: 13204 Rows   
####   - Number of Columns: 152 Columns 
####   - Data State: Requires PreProcessing 
## Instructions 
###  Stage 1: Data Cleaning
in this stage the goal is to clean the dataset so that we can have a dataset with meaningful information 
#### Original DataSet Information
![Df.info() Results](screenshots/86.png)
![Df.head() Results](screenshots/85.png)
![Df.describe() Results](screenshots/87.png)
#### Writing a list of column names to keep and renaming those columns to meaningful names
![New Column Names](screenshots/88.png)
![New Column Names](screenshots/89.png)
#### Renaming Division values to meaningful names 
![New Division Names](screenshots/92.png)
#### Extracting Time Analysis Data
![Time Analysis](screenshots/93.png)
#### Feature Engineering Season Column
![Season column engineering](screenshots/94.png)
#### Normalizing Probabilities to exclude bookmaker margin
![Normailized Probabilities](screenshots/95.png)

### Stage 2: Exploratory Data Analysis
#### Part 1: Descriptive statistics
 ##### 1. Numeric statistics:
           - FullTimeHomeGoals
           - FullTimeAwayGoals
           - HalfTimeHomeGoals
           - HalfTimeAwayGoals
           - HomeRedCards
           - AwayRedCards
           - Bet365_HomeWinOdds 
           - Bet365_DrawOdds 
           - Bet365_AwayWinOdds
  ![Numeric Statistics](screenshots/96.png)
 ##### 2. Frequency counts 
           - Matches per Division
           - Distribution of FullTimeResult
           -  Matches per season
           - Matches per weekday 
           -  Matches per month 
  ![Frequency Counts](screenshots/97.png)
  ![Frequency Counts](screenshots/98.png)
#### Part 2: Visualization of Distributions & Relationships among variables

##### 1. Distribution Visualizations:
- Histogram of Full-time goals scored (home and away)  
  ![Histogram of full-time goals scored](screenshots/99.png)

- Histogram of Betting odds  
  ![Histogram of betting odds (Home/Draw/Away)](screenshots/103.png)

- Bar plot for Count of matches per Division  
  ![Bar chart showing match count per Division](screenshots/104.png)

- Bar plot for Count of matches by FullTimeResult  
  ![Bar chart of match outcomes (H/D/A)](screenshots/105.png)

- Box plot for Goals scored by Division  
  ![Box plot comparing goals scored across Divisions](screenshots/106.png)

##### 2. Relationship Visualizations:
- Scatter plot to explore relationship between Home goals vs Away goals per match  
  ![Scatter plot: Home goals vs Away goals](screenshots/111.png)

- Scatter plot to explore relationship between Betting odds (e.g., HomeWinOdds) vs actual result (Raw and Implied probabilities)  
  ![Scatter plot of betting odds vs match result/probabilities](screenshots/113.png)

---

### Stage 3: Machine Learning

1. Select Features and Target  
   ![Feature selection and target variable definition](screenshots/114.png)

2. Split the Training and Test Datasets then train the model  
   ![Train-test split and model training](screenshots/115.png)

3. Evaluate the model  
   ![Model evaluation metrics (e.g., accuracy, confusion matrix)](screenshots/116.png)  
   ![Further model evaluation or ROC curve](screenshots/117.png)

### Stage 4: PowerBi Dashboard Creation
![Power Bi Dashboard](screenshots/118.png)
![Power Bi Dashboard](screenshots/119.png)
![Power Bi Dashboard](screenshots/120.png)
![Power Bi Dashboard](screenshots/121.png)
![Power Bi Dashboard](screenshots/122.png)
