# 📊 README – Real-Time Retail Analytics Dashboard  


Welcome to the **Real-Time Retail Analytics Dashboard** 🚀  

This project simulates a **live retail environment** where sales data is continuously generated, analyzed, and visualized in real-time. It provides:  

- 🔄 **Streaming synthetic retail transactions**  
- 📈 **Revenue & performance metrics across dimensions** (stores, products, categories, customers)  
- 🤖 **Anomaly detection with ML (Isolation Forest, DBSCAN)**  
- 🎨 **Interactive dashboards built with Streamlit & Plotly**   

## 🏗️ System Architecture  

### 🎨 Frontend Layer  
- 🖥️ **Streamlit Web Application**: Simple yet powerful dashboard  
- 📊 **Plotly Visualizations**: Interactive charts (time series, bar, scatter, anomaly heatmaps)  
- 📱 **Responsive Layout**: Sidebar for filters & configuration  
- 🔄 **Session State**: Keeps user interactions persistent  

### ⚙️ Data Generation Layer  
- 🏪 **Synthetic Retail Data** via **Faker**  
- 🎯 Configurable parameters (products, stores, customers)  
- 📦 Batch generation & sliding window (last 1000 transactions)  
- ⏱️ Adjustable frequency of data streaming  
![img alt](https://github.com/birukG09/Real-Time-Retail-Analytics/blob/e68541d87d4182ff11fe216df246c606066e7692/FireShot%20Capture%20006%20-%20Advanced%20Retail%20Analytics%20Platform_%20-%20%5B3680128b-5c43-4838-ba7a-2e7eab9595b4-00-3qhygwgjk12q4.worf.replit.dev%5D.png)
### 🧮 Analytics Engine  
- 📊 Multi-dimensional metrics (time, category, store, customer)  
- 📈 Revenue tracking & trend detection  
- 👥 Customer insights & transaction analysis  
- ⚡ Powered by **Pandas DataFrames** for efficient computation  

### 🤖 Anomaly Detection System  
- 🔍 **Isolation Forest** for ML-based anomaly scoring  
- 📏 Statistical thresholds for basic outlier detection  
- ⚙️ Configurable sensitivity (`contamination` factor)  
- 🧠 Feature engineering pipeline for improved detection  

### 🔄 Data Flow  
- 🧵 **Threading**: Background real-time data simulation  
- 🛠️ Event-driven dashboard refresh  
- 🗂️ Memory optimization with data pruning  
- 💾 Session-based state persistence  

---

## 📂 Project Structure  

```bash
Retail-Analytics-Dashboard/
│── 📜 README.md            # This README file
│── 📜 app.py               # Main Streamlit application
│── 📜 data_generator.py    # Synthetic retail data generator
│── 📜 analytics.py         # Core analytics & anomaly detection logic
│── 📜 visualization.py     # Plotly-based charts & visual components
│── 📜 requirements.txt     # Python dependencies
│── 📜 config.py            # Configuration (batch size, categories, etc.)
│── 📜 utils.py             # Helper functions
│── 📂 data/                # Temporary data storage
│── 📂 assets/              # Images, icons, static resources
│── 📂 notebooks/           # Jupyter notebooks for experimentation
│── 📂 tests/               # Unit tests
```

---

## ⚡ Getting Started  

### 🔧 Installation  

```bash
# Clone the repository
git clone https://github.com/birukG09/Retail-Analytics-Dashboard.git
cd Retail-Analytics-Dashboard

# Create and activate virtual environment
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

### 🚀 Run the Dashboard  

```bash
streamlit run app.py
```

Then open 👉 [http://localhost:8501](http://localhost:8501)  

---

## 📦 Dependencies  

- **Core**: 🐼 Pandas, 🧮 NumPy, 🎨 Streamlit, 📊 Plotly  
- **ML**: 🤖 scikit-learn (Isolation Forest, DBSCAN)  
- **Data Generation**: 🎭 Faker, 🕒 datetime, random  
- **System**: ⏱ threading, time, warnings  

---

## 🔥 Features  

✔️ Real-time data simulation  
✔️ Multi-dimensional revenue & sales analytics  
✔️ Anomaly detection with configurable thresholds  
✔️ Interactive dashboards (zoom, filter, drill-down)  
✔️ Synthetic yet **realistic** datasets for testing  

---

## 🔒 Security & Scalability Notes  

- 🔐 Runs locally by default – secure by design  
- 🛡️ For production: containerize with Docker + deploy behind authentication  
- ☁️ Can be scaled with **Kafka + Spark Streaming** replacing the Python generator for real event ingestion  
- 📡 Deploy on **AWS/GCP/Azure** with managed dashboards  
![img alt](https://github.com/birukG09/Real-Time-Retail-Analytics/blob/02bafbba6e8b7ca540b33ea5c328e593fa2199b3/20250901_1819_Real-Time%20Retail%20Dashboard_remix_01k42xmc36e6es2gnk2tept919.png)
---

## 🌍 Example Use Cases  

- 🏬 Retail store managers tracking daily performance  
- 📊 Data scientists testing real-time ML anomaly detection  
- 🎓 Students learning about **ETL, data pipelines, and analytics**  
- 🧑‍💻 Engineers prototyping real-time dashboards for IoT/finance/logistics  

---