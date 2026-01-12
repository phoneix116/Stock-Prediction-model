# 📈 Stock Price Prediction Using TensorFlow  

🔮 **A deep learning model built with TensorFlow to predict short-term stock prices.** This project uses historical stock price data and applies machine learning techniques to forecast future stock movements.  

---

## 🌟 Overview  

Predicting stock prices is a challenging task due to market volatility. This project leverages **deep learning** and **hyperparameter tuning** to build a robust stock prediction model. We use **Keras Tuner** to optimize neural network architecture for improved accuracy.  

📌 **Key Highlights:**  
- Uses **historical stock data** 📊  
- Applies **feature scaling** for better model performance 🔄  
- Implements a **deep learning model** with optimized layers 🤖  
- Leverages **Keras Tuner** for hyperparameter tuning 🎯  
- Provides **visualizations** to compare predicted vs. actual stock prices 📉  

---

## 🛠 Installation  

To get started, follow these steps:  

### 1️⃣ Clone the Repository  
```bash
git clone https://github.com/phoneix116/stock-price-prediction.git
cd stock-price-prediction
```

### 2️⃣ Install Dependencies  
Make sure you have Python installed, then run:  
```bash
pip install -r requirements.txt
```

### 3️⃣ Run the Model  
To train the model and make predictions, execute:  
```bash
open the jupyter notebook
```

---

## 📂 Dataset  

This model uses **Tata Global Beverages Limited** stock data. The dataset includes the following features:  

| Column | Description |
|--------|------------|
| `Date`  | Trading Date |
| `Open`  | Opening Price |
| `High`  | Highest Price |
| `Low`   | Lowest Price |
| `Close` | Closing Price |

Ensure your dataset follows a similar structure before training the model.  

---

## 🏗 Model Architecture  

🔍 **The deep learning model consists of:**  

✅ **Input Layer** → Takes `Open, High, Low, Close` values  
🔄 **Hidden Layers** → Fully connected dense layers (32-512 units)  
🎛 **Activation Function** → `ReLU` for hidden layers, `linear` for output  
⚙️ **Optimizer** → `Adam` (learning rate tuned with `Keras Tuner`)  
🎯 **Loss Function** → `Mean Squared Error (MSE)`  

---

## 🔥 Training Process  

The model is trained using a **split dataset strategy**:  
- **Training Set**: 80% of historical data  
- **Validation Set**: 10% for tuning  
- **Test Set**: 10% for final evaluation  

📌 **Optimization Features:**  
✅ `Keras Tuner` to select the best layer configurations  
✅ `EarlyStopping` to prevent overfitting  
✅ `MinMaxScaler` for feature normalization  

---

## 📊 Results & Visualization  

Once trained, the model predicts **next-day closing prices** based on historical trends.  

📉 **Predicted vs Actual Stock Prices:**  

![prediction_graph png](https://github.com/user-attachments/assets/eefe72a8-b6de-474b-ba47-3a70b7729631)

 
The model provides reasonable accuracy for **short-term forecasting**. Further improvements can be made by experimenting with:  
- More advanced neural network architectures (LSTM, GRU)  
- Larger datasets with different stocks  
- Incorporating external market indicators  

---

## 🚀 Hyperparameter Tuning with Keras Tuner  

**Keras Tuner** is used to optimize:  
- Number of **neurons** per layer  
- Number of **hidden layers**  
- **Learning rate** of optimizer  

The best configuration is selected dynamically based on **validation performance**.  

📌 To run the tuning process separately, execute:  
```bash
This process is integrated into the Jupyter Notebook
```

---

## 🏆 How to Contribute  

🚀 Want to improve the model? Follow these steps:  

1️⃣ **Fork the Repository**  
2️⃣ **Create a New Branch**  
```bash
git checkout -b feature-xyz
```
3️⃣ **Commit Your Changes**  
```bash
git commit -m "Added feature xyz"
```
4️⃣ **Push to GitHub**  
```bash
git push origin feature-xyz
```
5️⃣ **Open a Pull Request** 🎉  

---

## 📝 License  

📜 **MIT License** – Feel free to use and modify!  

---

## 🎯 Let's Predict the Market! 🚀  

If you found this project useful, please **⭐ Star** the repository! 😊  

---
