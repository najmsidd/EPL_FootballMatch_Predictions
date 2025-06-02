# EPL_FootballMatch_Predictions
This project leverages machine learning techniques to predict the outcomes of English Premier League (EPL) football matches. The model uses historical match data from the 2020-2021 and 2021-2022 seasons to train a Random Forest Classifier to predict match results. With a precision of 67.5%, this model provides an estimate of match outcomes based on features like the goals for, goals against, shots averaged etc which were feature engineered using thier rolling values to increase precision along with other features like the venue code, the opposition and even the hour and day of the week in which the team was playing

## Project Summary

- **Goal**: Predict the result of an EPL football match (Win/Loss/Draw).
- **Model Used**: `RandomForestClassifier` from Scikit-learn.
- **Data**: Match records from the 2020–2021 and 2021–2022 EPL seasons.
- **Achieved Precision**: 67.5% for predicting match outcomes.

---

## Features Used

The model uses a combination of engineered and contextual features such as:

- Rolling averages for:
  - Goals scored ("goals for")
  - Goals conceded ("goals against")
  - Shots taken and conceded
- Venue code (home/away)
- Opponent code
- Hour of the match
- Day of the week

These features help the model capture both team form and situational context of each match.

---

## Tools & Libraries

- Python
- Pandas
- Scikit-learn

---

## How It Works

1. **Data Preprocessing**: Raw EPL match data is cleaned and transformed.
2. **Feature Engineering**: Rolling averages and categorical encoding are applied.
3. **Model Training**: A Random Forest model is trained on the engineered features.
4. **Prediction & Evaluation**:
   - Predictions are made on test data.
   - Precision is calculated for model evaluation.

---

## Example Output

The model achieves a precision of 67.5% on match result predictions.  
Matches are predicted as Win or Loss/Draw based on team statistics and match context.

---

## Potential Improvements

- Incorporate player-level statistics such as injuries or performance ratings.
- Integrate betting odds or market sentiment as additional features.
- Experiment with advanced ensemble models like XGBoost or LightGBM.
- Explore time-series modeling techniques to track team momentum.

---
