# 🛢️Cooking Oil Price Forecasting using SARIMA and LSTM in Malaysia 


## 📈Project Overview 

This project focuses on forecasting cooking oil prices across all 14 states in Malaysia using two predictive models: **Seasonal Autoregressive Integrated Moving Average (SARIMA)** and **Long Short-Term Memory (LSTM) neural networks**. The study aims to provide accurate price forecasts to aid stakeholders such as policymakers, businesses, and consumers in making informed decisions. 

## 🔥Motivation 

Cooking oil prices in Malaysia exhibit significant fluctuations due to factors like global commodity market shifts, supply chain disruptions, and domestic economic policies. This project seeks to build a robust price prediction model leveraging historical price data to analyze seasonal trends and long-term dependencies. 

## 🗂️Data Source 

- **Dataset:** Historical cooking oil price data (2022-2023)
- **Source:** Malaysia Open Data Portal (data.gov.my)
- **Preprocessing:** Data cleaning, aggregation by state, handling missing values, and log transformation

## 🔄Project Workflow 
1. **Data Collection**: Gather historical price data from Malaysia Open Data Portal.
2. **Data Preprocessing**: Clean and transform data, ensuring consistency and handling missing values.
3. **Exploratory Data Analysis (EDA)**: Identify trends, seasonal patterns, and key insights.
4. **Model Development**: Implement SARIMA and LSTM models to forecast price trends.
5. **Model Evaluation**: Compare model performance using error metrics (MAE, RMSE, MAPE).
6. **Visualization & Interpretation**: Use Power BI to present results and insights.
7. **Deployment & Future Enhancements**: Explore improvements, including real-time updates.
   
    **Research Framework**
![Alt text](https://github.com/juna-99/Cooking-Oil-Price-Forecasting/blob/976ecee68c893c087ec4ae7783ab419f57820491/blob/Screenshot%202025-02-17%20104129.png)

    **Flowchart of The Proposed SARIMA Model**
![Alt text](https://github.com/juna-99/Cooking-Oil-Price-Forecasting/blob/976ecee68c893c087ec4ae7783ab419f57820491/blob/board-ridiculous-pickle%20(1).jpg)

    **Flowchart of The Proposed LSTM Model**
![Alt text](https://github.com/juna-99/Cooking-Oil-Price-Forecasting/blob/976ecee68c893c087ec4ae7783ab419f57820491/blob/board-ridiculous-pickle.jpg)

## 📊Results & Analysis 

### Model Performance
- **SARIMA Model**: Demonstrated superior performance in capturing seasonal trends with lower error rates.
- **LSTM Model**: Showed potential in handling complex patterns but exhibited higher variability.

### Error Metrics
| State        | SARIMA MAE | SARIMA RMSE | SARIMA MAPE | LSTM MAE | LSTM RMSE | LSTM MAPE |
|-------------|------------|-------------|-------------|----------|-----------|-----------|
| Johor       | 0.020      | 0.023       | 0.295%      | 0.320    | 0.365     | 3.710%    |
| Kedah       | 0.009      | 0.010       | 0.136%      | 0.244    | 0.287     | 2.946%    |
| Selangor    | 0.012      | 0.012       | 0.173%      | 0.273    | 0.319     | 3.236%    |

### Observations
- **SARIMA** consistently provided more stable and accurate predictions for states with strong seasonal patterns.
- **LSTM**, while capable of capturing complex relationships, had higher variability and was more sensitive to data fluctuations.
- **Final Recommendation**: SARIMA was more reliable for this dataset, but LSTM can be improved with further tuning and larger datasets. 

## 🛠️How to Use This Project 

1. Clone this repository
2. Install dependencies using `pip install -r requirements.txt`
3. Run EDA, SARIMA, and LSTM notebooks in `notebooks/`
4. Generate forecasts and compare results
5. Explore visualizations in Power BI 

## 🚀Future Improvements 

- Fine-tuning LSTM hyperparameters for better performance
- Integrating real-time price updates for continuous forecasting
- Expanding to other grocery price predictions 

## 🙌Acknowledgments 

Special thanks to **Ministry of Domestic Trade and Consumer Affairs (KPDN)** for providing the dataset. 



🏗️ Project Organization
------------

    ├── LICENSE
    ├── Makefile           <- Makefile with commands like `make data` or `make train`
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── docs               <- A default Sphinx project; see sphinx-doc.org for details
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jqp-initial-data-exploration`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    │
    ├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
    ├── src                <- Source code for use in this project.
    │   ├── __init__.py    <- Makes src a Python module
    │   │
    │   ├── data           <- Scripts to download or generate data
    │   │   └── make_dataset.py
    │   │
    │   ├── features       <- Scripts to turn raw data into features for modeling
    │   │   └── build_features.py
    │   │
    │   ├── models         <- Scripts to train models and then use trained models to make
    │   │   │                 predictions
    │   │   ├── predict_model.py
    │   │   └── train_model.py
    │   │
    │   └── visualization  <- Scripts to create exploratory and results oriented visualizations
    │       └── visualize.py
    │
    └── tox.ini            <- tox file with settings for running tox; see tox.readthedocs.io


--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
