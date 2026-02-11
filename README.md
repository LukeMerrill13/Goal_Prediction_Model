# Goal Prediction Model

This project builds a machine learning model to pedict the number of goals in League 1 and League 2 football matches. To do so, it follows a process of: data preparation, exploration, modelling, and simulation, to produce the most accurate model possible using the data provided. 

A short report and evlaution of the project is provided in `goal_prediction_model_report.pdf`

## Repository Structue
```
Goal_Prediction_Model/
│
├── data/
│ ├── league_one_and_two_data.csv
│ ├── prepared_data.csv
│ ├── model_predictions.csv
├── odds_data/
│   ├── E2_24 25.csv
│   ├── E2_25 26.csv
│   ├── E3_24 25.csv
│   └── E3_25 26.csv
│
├── python_notebooks/
│ ├── data_preparation.ipynb
│ ├── exploratory_data_analysis.ipynb
│ ├── model_development.ipynb
│ └── betting_simulation.ipynb
│
├── goal_prediction_model_report.pdf
└── README.md
```
## Running the Project

The project can be ran by following the steps below:

### 1. Clone the repository

```bash
git clone https://github.com/LukeMerrill13/Goal_Prediction_Model.git
cd Goal_Prediction_Model
```
### 2. Add the required data

Two datasets are used in this project. The first conatains match outcome and xG data on League 1 and League 2 matches between the 2017/18 and 2025/26 seasons. The second contains similar match result data alongside historical odds on the over/under 2.5 goals market. This data was sourced from wwww.football-data.co.uk.
Add the data files into the `data/` directory:

- `league_one_and_two_data.csv`
- `odds_data.csv`

### 3. Execute the notebooks in order

1. `data_preparation.ipynb`
    Prepares the data for exploratory analysis and model development.
    Produces `prepared_data.csv' for use in subsequent notebooks
2. `exploratory_data_analysis.ipynb`
    Looks for patterns in the data which might inform modelling decisions.
3. `model_development.ipynb`
    Develops the goal prediction model. Creates `model_predictions.csv` which is used in the subsequet notebook.
4. `betting_simulation.ipynb`  
