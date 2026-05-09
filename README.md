# Capstone Project Module 3 - Saudi Arabia Used Cars Price Prediction
**Nama:** Azhar Zahid Misbahuddin  
**Batch:** JCDSOHAM-06 Purwadhika  

### 1. Business Problem
Dealer mobil bekas di Arab Saudi kesulitan menentukan harga jual yang optimal. Project ini bertujuan membangun model Machine Learning untuk memprediksi harga mobil bekas.

### 2. Dataset
Dataset: Saudi Arabia Used Cars, 3,767 baris setelah cleaning.  
Fitur utama: `Car_Age`, `Engine_Size`, `Mileage`, `Type`, `Make`.  
Target: `Price` dalam SAR.

### 3. Model Performance
| Metric | Score |
| --- | --- |
| R² Score | 0.8196 |
| RMSE | 27,944.72 SAR |
| MAE | 14,947.74 SAR |

Model Random Forest mampu menjelaskan 81.96% variasi harga mobil.

### 4. How to Use
```python
import pickle
import pandas as pd

# Load model
with open('model.pkl', 'rb') as file:
    model = pickle.load(file)

# Prediksi harga mobil baru
# model.predict(data_baru)
