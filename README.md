# 📊 Gold Price Forecasting using RNN

---

## 📄 Project Description  
This project focuses on forecasting gold prices using a Recurrent Neural Network (RNN) based deep learning model.  
The dataset contains historical daily gold price data. The goal is to predict future gold prices based on past trends.

---

## 🗂 Dataset  
The dataset contains gold price data with multiple features. For this project, the main feature used is the **closing price**.

- **Source**: [Kaggle – Gold Price Data](https://www.kaggle.com/datasets/sid321axn/gold-price-data)  
- **File Name**: `gold_price_data.csv`  
- **Preprocessing Steps**:
  - Convert the `Date` column to datetime format.
  - Set `Date` as index.
  - Normalize data using `MinMaxScaler`.
  - Create time windows of 20 days to predict the next day.

---

## 🔧 Technologies and Tools Used  
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Scikit-learn  
- TensorFlow / Keras  

---

## ⚙️ Project Workflow

1. **Data Loading**: Load and inspect the dataset from CSV.  
2. **Datetime Processing**: Convert date strings to datetime objects and set as index.  
3. **Data Normalization**: Use MinMaxScaler to scale price values between 0 and 1.  
4. **Window Creation**: Build sequences of 20 days to predict the 21st day price.  
5. **Train-Test Split**: Use 80% of the data for training, 20% for testing.  
6. **Model Building**: Sequential model with two `SimpleRNN` layers and a dense output layer.  
7. **Model Compilation**: Use MSE loss function and Adam optimizer.  
8. **Training**: Train the model and monitor validation loss.  
9. **Evaluation**: Predict on test data and calculate MAE and MSE.  
10. **Visualization**: Plot real vs predicted prices.

---

## 📈 Model Architecture Summary  
- **SimpleRNN Layer** with 64 units and ReLU activation.  
- **SimpleRNN Layer** with 32 units.  
- **Dense Output Layer** with 1 unit for regression.  
- **Loss Function**: Mean Squared Error (MSE)  
- **Optimizer**: Adam

---

## 🚀 How to Run  

1. Install required libraries if not already installed:  
   ```bash
   pip install pandas numpy matplotlib scikit-learn tensorflow

2. Place the dataset (gold_price_data.csv) in your working directory.

3. Run the Jupyter Notebook:
forecasting_gold.ipynb

4. The model will be trained, evaluated, and the predictions plotted for comparison.

## 👨‍💻 About the Developer
This project was developed by Abdulaziz Mohammed Dahan.
Thank you for checking out this project!
