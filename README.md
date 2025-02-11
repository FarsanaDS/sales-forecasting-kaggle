# Kaggle competition
📊 Sales Forecasting - Kaggle Competition

🚀 Predicting future sales using advanced machine learning techniques! This project was built for a Kaggle competition, applying XGBoost and LightGBM to forecast sales.

---

📌 Project Overview

Sales forecasting is a critical problem in retail. This project uses historical sales data along with feature engineering and machine learning models to predict future sales.

🔹 Dataset: Provided in the Kaggle competition.
🔹 Goal: Predict the sales_hat (future sales) for given items.
🔹 Challenge: Handling missing data, feature engineering and hyperparameter tuning to improving accuracy.

---

📂 Dataset Details

The dataset includes sales transactions with columns like:
id: Unique identifier for the item and date.
date: Transaction date.
sales: Number of units sold.
sell_price_main: Selling price of the item.
discounts: Various types of discounts applied.
holidays: Whether the date is a holiday or not.

🔹 Train Set: sales_train.csv (4M+ rows)
🔹 Test Set: sales_test.csv (No sales column, to be predicted)

---

🛠 Techniques Used

⿡ Feature Engineering

✅ Date Features: Extracted year, month, day, weekday, is_weekend, quarter
✅ Lag Features: sales_lag_1, sales_lag_7, sales_lag_30 (previous sales history)
✅ Rolling Statistics: sales_ma_7, sales_ma_30 (moving averages)
✅ Exponential Moving Average (EMA): sales_ema_7, sales_ema_30
✅ Price Features: price_change, price_elasticity
✅ Stock Availability: is_out_of_stock, availability
✅ Discount Effects: total_discount, discount_rate, discount_per_order

⿢ Model Training

✅ XGBoost with Hyperparameter Tuning (RandomizedSearchCV)
✅ LightGBM for Speed and Performance

⿣ Hyperparameter Tuning
Used RandomizedSearchCV to optimize:
n_estimators
max_depth
learning_rate
subsample
colsample_bytree
gamma, reg_alpha, reg_lambda

---

📈 Model Performance

🏆 Final R² Score:
Train: 0.9975
Test: 0.9974

📉 Competition Score: 77.97917

---

📌 How to Run the Code

⿡ Clone the repository:

git clone https://github.com/FarsanaDS/sales-forecasting-kaggle.git
cd sales-forecasting-kaggle

⿢ Install dependencies:

pip install -r requirements.txt

⿣ Run the notebook:

jupyter notebook

⿤ Train the model and generate predictions.
⿥ Save submission file:
submission.to_csv("submission.csv", index=False)

---

🚀 Future Improvements

🔹 Try LSTMs or Transformers for time-series forecasting.
🔹 Use external data sources like economic indicators.
🔹 Apply feature selection for reducing dimensionality.

---

📝 Author

👩‍💻 Farsana
💼 Aspiring Senior Data Scientist
📌 From Malappuram, Kerala
🔗 www.linkedin.com/in/farsana-thasnem-pa-03553631a | https://github.com/FarsanaDS

---

⭐ Contributions & Feedback

Feel free to fork the repo, raise issues, or suggest improvements! 🚀🔥

---


