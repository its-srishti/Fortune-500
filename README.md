# Fortune 500 Revenue Forecasting
## It applies **time-series forecasting models** to predict the future revenues of Fortune 500 companies using more than **33,000 data points**. The analysis leverages both traditional statistical methods and deep learning models to benchmark forecasting performance.  

### 📂 Project Structure
- `Fortune_500_Analytics.ipynb` → Jupyter notebook with the complete analysis, model training, and results.
- `preprocessed_fortune500_data.csv` → Cleaned dataset used for training and testing.
- `requirements.txt` → List of dependencies (for reproducibility).

---

### ⚙️ Methodology
1. **Data Preparation**  
   - Preprocessed the raw revenue data to handle missing values, ensure stationarity, and split into training/testing sets.  

2. **Models Implemented**  
   - **ARIMA** (AutoRegressive Integrated Moving Average)  
   - **SARIMA** (Seasonal ARIMA)  
   - **LSTM** (Long Short-Term Memory Neural Network)  

3. **Evaluation**  
   - Compared model performance using standard metrics such as MAPE/RMSE.  
   - **LSTM consistently outperformed ARIMA and SARIMA**, capturing complex nonlinear trends more effectively.  

---

### 📊 Key Findings
- Statistical models like ARIMA and SARIMA provided reasonable short-term forecasts but struggled with longer horizons.  
- LSTM captured long-term patterns and provided the **best forecast accuracy** among the three models with an MSE of 0.01.  
- Demonstrates the growing advantage of deep learning methods for financial time-series forecasting.  

---

### 🚀 Future Scope
- Incorporate **external macroeconomic indicators** (e.g., interest rates, GDP growth, inflation) as exogenous variables to improve accuracy.  
- Explore more advanced models like **Transformer-based architectures** (e.g., Temporal Fusion Transformer).  
- Extend the analysis to **profitability, costs, and sector-level trends** for richer insights.  
- Build an **interactive dashboard** for real-time forecasting.  

---

### ⚠️ Caveats
- **Data Limitations**: Forecasts depend heavily on historical patterns. Sudden shocks (e.g., pandemics, policy changes, market crashes) are not captured. COVID-19 revenue dip could not be predicted.
- **Model Assumptions**: ARIMA assumes stationarity; LSTMs require careful tuning and large datasets.  
- **Interpretability**: Deep learning models (like LSTM) are less interpretable than traditional statistical approaches.  

---

### 🛠️ Installation & Usage
Clone this repository and install the requirements:
```bash
git clone https://github.com/its-srishti/fortune500-revenue-forecasting.git
cd fortune500-revenue-forecasting
pip install -r requirements.txt
