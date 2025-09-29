# 🎧 Spotify User Churn Analysis

This project analyzes user behavior on a music streaming platform (similar to Spotify) to understand what drives churn and predict whether a user is likely to stop using the service.

---

## 📁 Files in This Repository

| File | Description |
|------|-------------|
| `spotify_users.csv` | The dataset containing user listening behavior and churn labels |
| `model_building.ipynb` | Notebook for preprocessing, modeling (Logistic Regression, Random Forest, SMOTE) |
| `data_analysis.ipynb` | Notebook for exploratory data analysis (EDA) and visual insights |
| `README.md` | This documentation |
| `requirements.txt` | (Optional) Python packages required to run the notebooks |

---

## 📊 Dataset Description

The dataset (`spotify_users.csv`) includes **8,000 user records** with the following columns:

| Column | Description |
|--------|-------------|
| `user_id` | Unique user ID |
| `gender` | Gender of the user |
| `age` | User’s age |
| `listening_time` | Minutes spent listening per day |
| `songs_played_per_day` | Songs played daily |
| `skip_rate` | Fraction of songs skipped |
| `device_type` | Device used (Mobile/Desktop/Web) |
| `ads_listened_per_week` | Number of ads heard per week |
| `offline_listening` | Whether offline listening is enabled |
| `subscription_type` | Free, Premium, Student, or Family |
| `is_churned` | **Target** — whether the user churned (1 = churned, 0 = retained) |

---

## 🧪 Project Objectives

- **Analyze user behavior patterns** between churned and retained users
- **Build machine learning models** to predict churn
- **Identify key features** driving user churn
- **Generate actionable business insights** to improve user retention

---

## 📈 Analysis Performed

In `data_analysis.ipynb`:

- Class imbalance and churn rate calculated
- Churn trends by gender, age, device, subscription type
- Behavior insights: skip rate, listening time, ad exposure
- Feature correlations visualized
- Summary statistics interpreted to draw conclusions

---

## 🤖 Models Used

In `model_building.ipynb`:

- Logistic Regression (with and without class balancing)
- Random Forest (with class_weight='balanced')
- SMOTE oversampling to fix class imbalance
- XGBoost (optional)
- Evaluation with precision, recall, F1-score, classification reports


---

## 🔍 Key Insights

- **Churn Rate**: ~26% of users churn
- **Subscription Type**: Free and Student plans have higher churn
- **Skip Rate**: High skip rates strongly correlate with churn
- **Ads**: Users exposed to many ads are more likely to churn
- **Offline Listening**: Correlates with higher retention
- **Feature Importance**: Skip rate, listening time, and subscription type are top predictors

---


