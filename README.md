# 🚗 Used Car Price Prediction

Machine learning project to predict the market price of used cars for Rusty Bargain. The goal was to develop a model that is not only accurate (minimizing RMSE) but also efficient in terms of training time and prediction speed.

---

## 📌 Objective

- Predict car resale value based on historical and technical attributes
- Compare performance between baseline linear models, decision trees, random forests, and gradient boosting (LightGBM, CatBoost)
- Select the most practical and performant model for deployment in a mobile app

---

## 📊 Dataset Description

- `DateCrawled`: Profile scraped date
- `VehicleType`: Car body type
- `RegistrationYear`: Vehicle registration year
- `Gearbox`: Transmission type
- `Power`: Horsepower (in HP)
- `Model`: Car model
- `Mileage`: Vehicle mileage in km
- `RegistrationMonth`: Month of registration
- `FuelType`: Type of fuel
- `Brand`: Vehicle brand
- `NotRepaired`: Repair status (yes/no)
- `DateCreated`: Profile creation date
- `NumberOfPictures`: Number of images uploaded
- `PostalCode`: User location code
- `LastSeen`: Last user activity
- `Price`: **Target variable** – listed price in euros

---

## 🧪 Models Compared

1. **Linear Regression** – sanity baseline
2. **Decision Tree Regressor**
3. **Random Forest Regressor** – tuned with `GridSearchCV`
4. **LightGBM Regressor** – tested with learning rate, depth
5. **CatBoost Regressor** – fast training and built-in categorical support

---

## 🧠 Evaluation Metrics

- **Root Mean Squared Error (RMSE)** – Main metric
- **Training Time**
- **Prediction Time**

---

## 📈 Key Insights

- Random Forest and CatBoost yielded the best balance between accuracy and prediction speed
- Linear Regression was the slowest and least accurate (as expected)
- LightGBM offered competitive performance with careful tuning
- CatBoost outperformed on categorical-heavy data with minimal preprocessing

---

## 📁 Project Structure

```
used-car-price-prediction/
│
├── used_car_price_modeling.ipynb
├── car_data.csv
├── requirements.txt
└── README.md
```

---

## 🛠️ Tools & Libraries Used

- Python
- pandas, numpy
- scikit-learn
- LightGBM
- CatBoost

---

## ✅ Status

✔️ Project completed as part of the **TripleTen Bootcamp** – Sprint: *Gradient Boosting vs. Forests vs. Linear Regression*

---

## 📌 Author

David Villanueva  
[LinkedIn](https://www.linkedin.com/in/david-villanueva-59659727)  
[GitHub](https://github.com/lolapaul)
