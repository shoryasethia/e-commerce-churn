# Predicting User Churn for an E-commerce Platform

## Report
Work report containing Feature Engineering, Churn Definition & its Reasoning, Predictive Modeling and How to incorporate all this to get some Business Insights and direction to design suitable campaigns are included in this [Report](https://github.com/shoryasethia/e-commerce-churn/blob/main/Report.pdf).

## Get Started
Clone the Repository:
```bash
git clone https://github.com/shoryasethia/e-commerce-churn.git
cd e-commerce-churn
```
Install Dependencies:
```bash
pip install -r requirements.txt
```
## Datasets
Given and derived datasets are in `data/`

## Features
Defination of extracted features can be found in `FEATURES.md`

## To replicate results and data
1. Firstly run `events_eda.ipynb` to get overview of the data, some plots and values which would help in understanding the data
2. Then run, `events_clean.ipynb` to handle missing values in `events.csv`, this will generate `evemts_cleaned.csv`
3. Then run `events_features.ipynb` to extract meaningful features; `events_features.csv` and `events_features_extended.csv` will be generated
4. Next, run `churn.ipynb` to generate `user_churn_analysis.csv` and `user_churn_risk_analysis.csv`
5. Run `churn_eda.ipynb` to extract and get insights for business modelling, predictive modelling and intution for campaigns
6. To get `events_with_churn_score.csv` run `events_with_churn.ipynb`
7. To train Random Forest and Gradient Boost to predict which user(s) is/are likely to churn, run `model.ipynb`
8. To train Random Forest to predict which user(s) risk category, run `risk_category.ipynb`

## Brief Business Recommednations and Campaigns
![business-recommendations-mermaid](https://github.com/shoryasethia/e-commerce-churn/blob/main/business-recommendations.png)

## References
Helpful resources like papers and articles are added in work report, but some of them are added in `papers/` as well

> For any questions, feel free to open an [issue](https://github.com/shoryasethia/e-commerce-churn/issues) or reach out at [shoryasethia4may@gmail.com](mailto:shoryasethia4may@gmail.com)


