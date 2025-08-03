#Football Data Machine Learning
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
![Df.info() Results](screenshots/Screenshot (86))
![Df.head() Results](screenshots/Screenshot (85))
![Df.describe() Results](screenshots/Screenshot (87))
#### Writing a list of column names to keep and renaming those columns to meaningful names
![New Column Names](screenshots/Screenshot (88))
![New Column Names](screenshots/Screenshot (89))
#### Renaming Division values to meaningful names 
![New Division Names](screenshots/Screenshot (92))
#### Extracting Time Analysis Data
![Time Analysis](screenshots/Screenshot (93))
#### Feature Engineering Season Column
![Season column engineering](screenshots/Screenshot (94))
#### Normalizing Probabilities to exclude bookmaker margin
![Normailized Probabilities](screenshots/Screenshot (95))

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
  ![Numeric Statistics](screenshots/Screenshot (96))
 ##### 2. Frequency counts 
           - Matches per Division
           - Distribution of FullTimeResult
           -  Matches per season
           - Matches per weekday 
           -  Matches per month 
  ![Frequency Counts](screenshots/Screenshot (97))
  ![Frequency Counts](screenshots/Screenshot (98))
#### Part 2: Visualization of Distributions & Relationships among variables

##### 1. Distribution Visualizations:
- Histogram of Full-time goals scored (home and away)  
  ![Histogram of full-time goals scored](screenshots/Screenshot(99))

- Histogram of Betting odds  
  ![Histogram of betting odds (Home/Draw/Away)](screenshots/Screenshot(103))

- Bar plot for Count of matches per Division  
  ![Bar chart showing match count per Division](screenshots/Screenshot(104))

- Bar plot for Count of matches by FullTimeResult  
  ![Bar chart of match outcomes (H/D/A)](screenshots/Screenshot(105))

- Box plot for Goals scored by Division  
  ![Box plot comparing goals scored across Divisions](screenshots/Screenshot(106))

##### 2. Relationship Visualizations:
- Scatter plot to explore relationship between Home goals vs Away goals per match  
  ![Scatter plot: Home goals vs Away goals](screenshots/Screenshot(111))

- Scatter plot to explore relationship between Betting odds (e.g., HomeWinOdds) vs actual result (Raw and Implied probabilities)  
  ![Scatter plot of betting odds vs match result/probabilities](screenshots/Screenshot(113))

---

### Stage 3: Machine Learning

1. Select Features and Target  
   ![Feature selection and target variable definition](screenshots/Screenshot(114))

2. Split the Training and Test Datasets then train the model  
   ![Train-test split and model training](screenshots/Screenshot(115))

3. Evaluate the model  
   ![Model evaluation metrics (e.g., accuracy, confusion matrix)](screenshots/Screenshot%20(116))  
   ![Further model evaluation or ROC curve](screenshots/Screenshot(117))

### Stage 4: PowerBi Dashboard Creation

