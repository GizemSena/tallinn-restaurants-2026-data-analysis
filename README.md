# 🍽️ Tallinn Restaurants Analysis (2026)

## 📌 Project Overview

This project analyzes restaurant data from Tallinn in 2026 to understand key factors that influence restaurant quality and customer experience.

The analysis focuses on:

* Food quality 🍴
* Service quality 🤝
* Atmosphere 🌆
* Pricing 💰
* Overall restaurant performance ⭐

---

## 📊 Dataset Information

The dataset contains **97 restaurants** with the following features:

* `Restaurant` – Name of the restaurant
* `URL` – Website link (if available)
* `Address` – Location details
* `Cuisine` – Type of cuisine
* `Price_category` – Pricing level
* `Atmosphere` – Atmosphere rating
* `Food` – Food quality rating
* `Service` – Service quality rating
* `Weighted_score` – Overall score
* `Latitude` – Geographic coordinate
* `Longitude` – Geographic coordinate

---

## ⚙️ Data Processing

### Data Cleaning

* Missing values in the `URL` column were handled
* Data types were verified and standardized

### Feature Engineering

* **Score_Diff** = Food − Service
* **Avg_Quality** = (Food + Service + Atmosphere) / 3

These features help better understand differences in restaurant performance.

---

## 📈 Exploratory Data Analysis (EDA)

The following analyses were performed:

* Distribution of cuisines
* Distribution of price categories
* Analysis of Food, Service, and Atmosphere scores
* Identification of top-performing restaurants
* Relationship between Food and Service scores
* Impact of pricing on overall quality
* Correlation analysis between numerical features
* Geographic distribution of restaurants

---

## 🔍 Key Insights

* Restaurants with higher prices tend to have better overall quality
* Food quality has the strongest influence on the overall score
* Some restaurants have high food ratings but relatively lower service ratings
* Most restaurants fall within mid-to-high score ranges
* Certain cuisines consistently outperform others in average ratings

---

## 🤖 Machine Learning Model

A **Random Forest Regressor** was used to predict restaurant scores.

### Steps:

* Categorical features encoded using Label Encoding
* Data split into training and testing sets (80/20)
* Model trained to predict `Weighted_score`

### Result:

* The model successfully captured relationships between quality metrics and overall scores

---

## 🛠️ Technologies Used

* Python 🐍
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

---

## 🚀 Future Improvements

* Apply advanced models (XGBoost, LightGBM)
* Build an interactive map visualization
* Include customer review data
* Perform sentiment analysis on restaurant reviews

---

## 📎 Conclusion

This analysis shows that restaurant success in Tallinn is primarily driven by food quality, followed by service and atmosphere. Pricing also plays an important role, often reflecting overall quality.

---

## 👩‍💻 Author

Gizem Sena ÇENGEL
Computer Engineer
Data Science & AI Enthusiast 🚀
