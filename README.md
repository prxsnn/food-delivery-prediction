#Food Delivery Time Prediction

This project predicts how long a food delivery will take based on various real-world factors like distance, weather, traffic, and restaurant rating. It uses a simple linear regression model to estimate delivery time in minutes.

---

#Objective

To build a basic predictive model that estimates food delivery time using structured delivery-related data. This can help food platforms better manage delivery logistics and customer expectations.

---

#Dataset

The dataset contains 10 sample entries (mock data) with the following features:

- `Restaurant_Rating` – Average customer rating of the restaurant  
- `Delivery_Distance_km` – Distance to the customer in kilometers  
- `Delivery_Person_Age` – Age of the delivery personnel  
- `Traffic_Conditions` – Traffic level during delivery (`Low`, `Medium`, `High`)  
- `Weather_Conditions` – Weather conditions (`Clear`, `Cloudy`, `Rainy`)  
- `Delivery_Time` – Target variable (in minutes)

> Note: This is a compact, mock dataset created for learning/demo purposes.

---

## Project Workflow

1. **Data Exploration & Cleaning**
   - Checked for null values and basic statistics.
   - Dataset had no missing values.

2. **Preprocessing**
   - One-hot encoded categorical columns: `Traffic_Conditions` and `Weather_Conditions`.

3. **Modeling**
   - Model: `LinearRegression` from `sklearn`
   - Split: 80/20 train-test split
   - Target: `Delivery_Time`

4. **Evaluation**
   - Metric: `Mean Absolute Error (MAE)`
   - Final MAE on test data: ~**9.97 minutes**

5. **Visualization**
   - Plotted distribution of prediction error to check for bias and variance.

---

#Tech Stack

- Python 3
- Pandas
- Matplotlib / Seaborn
- Scikit-learn

---

#Results

| Metric | Value |
|--------|-------|
| MAE (Test Set) | **9.97 minutes** |

This means on average, the model is off by ~10 minutes in its delivery time predictions.

---

#How to Run

1. Clone this repo or open the notebook in Google Colab.
2. Make sure `food_delivery.csv` is uploaded in your session.
3. Run each cell to preprocess data, train the model, and evaluate results.

---

#Possible Improvements

- Increase dataset size for better generalization.
- Try advanced models like Random Forest or Gradient Boosting.
- Add new features like delivery time of day, weekend indicator, order size, etc.
- Use real-time traffic/weather APIs for live predictions.

---

#Author

Prasann Arora  
M.Tech in Data Science, IIT Guwahati  
