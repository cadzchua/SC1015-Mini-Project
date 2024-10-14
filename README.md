# SC1015 Mini-Project: Titanic Survival Analysis

## Team Members

- **Cadden Chua**
- **Chooi Li Hang**
- **Tristan Ng**

## Overview

This mini-project focuses on analysing the survival rates of passengers aboard the Titanic using data from Kaggle. The project aims to uncover insights regarding factors that influenced survival during the tragic sinking of the ship.

## Motivation

- **Historical Significance**: The Titanic disaster is one of the most infamous maritime tragedies in history. Analysing this event provides insights into historical societal norms, such as class disparity and gender roles, and how they influenced survival rates.

- **Real-World Relevance**: The Titanic disaster serves as a case study for understanding human behavior in crises. Investigating survival rates can provide insights applicable to modern emergency management, helping to inform policies and procedures for future disasters.

## Objectives

- To explore the dataset and conduct exploratory data analysis (EDA) to identify key factors affecting survival.
- To visualise the data through various plots, providing insights into the relationships between different variables.
- To formulate and answer specific research questions related to passenger survival.
- To develop predictive models for estimating survival outcomes.

## Dataset

The project utilises the Titanic dataset, which includes various features of the passengers such as:

- Passenger Class (`Pclass`)
- Age (`Age`)
- Gender (`Sex`)
- Fare (`Fare`)
- Family Size (`SibSp`, `Parch`)
- Embarkation Point (`Embarked`)

## Key Questions

1. What is the relationship between passenger class and survival?
2. How does age impact survival rates?
3. Is there a correlation between gender and survival?
4. What is the relationship between family size (`SibSp`, `Parch`) and survival?
5. Does the embarkation point (`Embarked`) affect survival chances?

## Data Preparation and Cleaning

We addressed missing data in columns such as `Age` and `Embarked` using imputation techniques. Categorical variables such as `Sex` and `Embarked` were encoded using one-hot encoding, while numerical features like `Fare` were scaled for consistency.

## Exploratory Data Analysis (EDA)

Our EDA focused on understanding the relationships between different features and survival outcomes. We utilised:

- **Correlation Heatmap**: This visualises correlations between numerical features and survival, showing that `Pclass`, `Sex`, and `Fare` have strong relationships with survival.
- **Bar Plots and Histograms**: We explored survival rates based on passenger class, gender, age, family size, and embarkation point.
- **Box Plots**: These plots helped us understand the distribution of features like `Age` and `Fare` across survivors and non-survivors.

## Machine Learning Techniques

We employed the following machine learning models to predict survival:

- **Logistic Regression**: A baseline model used to predict survival based on key features.
- **Decision Tree Classifier**: Used to model feature importance and visualise decision-making processes.
- **Random Forest Classifier**: An ensemble model to improve predictive accuracy.
- **XGBoost**: A gradient boosting algorithm for optimising predictions.

Each model was evaluated using cross-validation, accuracy scores, confusion matrices, and classification reports to determine the best performing model.

## Results and Insights

- **Key Factors for Survival**:
  - Passengers in first class had a significantly higher chance of survival.
  - Women were more likely to survive than men, especially those in higher age groups.
  - Fare and embarkation point also played a role in survival likelihood.
- **Model Performance**:
  - The Random Forest model achieved the highest accuracy, followed by Logistic Regression and Decision Tree models.
  - Feature importance analysis showed `Pclass`, `Sex`, and `Fare` as the most significant predictors of survival.

## Individual Contributions

Each team member contributed to data cleaning, EDA, and model development. Specific roles included:

- **Cadden Chua**: Data cleaning, EDA visualisations, feature extraction, modelling and slides.
- **Chooi Li Hang**: Data cleaning, EDA visualisations, feature importance, modelling and slides
- **Tristan Ng**: Data cleaning, EDA visualisations and slides.

## Installation

To run the project, ensure you have the following libraries installed:

```bash
pip install requirements.txt
```

## Usage

1. **Clone the repository**:
   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```
2. Open the Jupyter notebook to view the analysis and visualisations.

## Contributing

Contributions are welcome! Please fork this repository, make your changes, and submit a pull request.

1. Star and fork the repository.
2. Create a new branch: `git checkout -b my-feature-branch`
3. Make your changes.
4. Commit your changes: `git commit -m 'Add some feature'`
5. Push to the branch: `git push master my-feature-branch`
6. Open a pull request.

## References

- [Kaggle Titanic Dataset](https://www.kaggle.com/c/titanic)

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Authors

The portfolio project is maintained by cadzchua, henrychooi and natsirt04.
