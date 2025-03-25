# 📈 Stock Prediction Model using TensorFlow

A deep learning model built using **TensorFlow and Keras** to predict stock prices based on historical data. The model takes **6 feature inputs** and uses **Dense layers** to make predictions.

---

## 🚀 Features  
- 📊 Uses deep learning (**Dense layers**) for stock price prediction  
- 🔢 Trained on **6 input features** to analyze market trends  
- 🎯 Optimized with **Mean Squared Error (MSE) loss function**  
- 📈 Generates **real-time predictions** for stock movements  

---

## 📦 Installation  

### Clone the repository:  
```bash
git clone https://github.com/your-username/stock-prediction-tensorflow.git
cd stock-prediction-tensorflow
```

### Install dependencies:  
```bash
pip install -r requirements.txt
```

### Run the training script:  
```bash
python train.py
```

---

## 🔧 Model Architecture  

```python
model = keras.Sequential([
    keras.layers.Input(shape=(X_train.shape[1],)),
    keras.layers.Dense(128, activation='relu'),
    keras.layers.Dense(64, activation='relu'),
    keras.layers.Dense(32, activation='relu'),
    keras.layers.Dense(16, activation='relu'),
    keras.layers.Dense(1, activation='linear')  # Output is probability of price going UP
])
```

- **Loss Function:** Mean Squared Error (MSE)  
- **Metrics:** Mean Absolute Error (MAE)  

---

## 📊 Usage  

### Prepare your dataset:  
Ensure `X_train` and `y_train` are preprocessed.  

### Train the model:  
```python
model.fit(X_train, y_train, epochs=75, batch_size=16, validation_data=(X_val, y_val))
```

### Make predictions:  
```python
predictions = model.predict(X_test)
print(predictions)
```

---

## 📈 Example Prediction  
Example output from the model:  
```bash
Predicted Stock Price: 125.47
```

---

## 🛠 Technologies Used  
- 🐍 **Python**  
- 🤖 **TensorFlow/Keras**  
- 📊 **NumPy & Pandas**  
- 📉 **Matplotlib & Plotly**  

---

## 🏗 Contributing  
Pull requests are welcome! To contribute:  

1. **Fork the repo**  
2. **Create a new branch:**  
   ```bash
   git checkout -b feature-name
   ```
3. **Commit your changes:**  
   ```bash
   git commit -m "Added feature XYZ"
   ```
4. **Push to GitHub and open a PR:**  
   ```bash
   git push origin feature-name
   ```

---

## 📜 License  
This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

