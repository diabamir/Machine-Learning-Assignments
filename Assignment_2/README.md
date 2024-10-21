# Assignment 2: Predicting Football Match Outcomes

### Data

This dataset contains a comprehensive record of international football results spanning from 1872 to 2017. It includes match outcomes between national teams, providing a historical view of international football performance.

**Dataset columns**:
- `results.csv`: Contains match details (date, teams, scores, etc.).
- `shootouts.csv`: Information about matches decided by penalty shootouts.
- `goalscores.csv`: Contains the scores and goal times in international games.

---

### Tasks:

#### Section A - Data Exploration & Visualization 
- Explore the data using tables and visualizations. 
- Create informative plots with titles, axis labels, and a legend.
- Provide a short description of key observations from each plot.

#### Section B - Data Preprocessing 
- Perform feature engineering to create the following features:
  - **Home team won**: A boolean feature representing whether the home team won (use shootouts.csv for drawn matches).
  - **Home team win rate**: Percentage of matches the home team won up to that point.
  - **Away team win rate**: Percentage of matches the away team won up to that point.
  - **Home team average goals**: Average number of goals the home team has scored up to that point.
  - **Away team average goals**: Average number of goals the away team has scored up to that point.
  - **Additional features**: Create at least six more features of your choosing.

- Apply imputation, transformation, and feature selection methods as needed.

#### Section C - Home Team Winning Prediction 
- Use at least three machine learning models to predict whether the home team won (use `Home_team_won` feature).
- Perform hyperparameter tuning and report the model's performance.
- Present the models' results in a plot and compare them.

#### Section D - Clustering 
- Create a new dataset where each row represents a team and features describe their game history.
- Apply at least two clustering algorithms (e.g., K-Means, GMM) on this data.
- Perform parameter tuning and identify important features.
- Use a method to estimate the quality of clusters and visualize the results.


