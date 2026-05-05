# 🚦 Real-Time Traffic Congestion Analytics

## Using Big Data Streaming Pipeline

---

## 📌 Project Overview

This project demonstrates a real-time traffic monitoring system built using a big data streaming pipeline.
It simulates live traffic data, processes it using PySpark, and visualizes insights through a Streamlit dashboard.

### 🔍 The system helps in:

* 🚗 Detecting traffic congestion in real time
* 📊 Visualizing traffic patterns
* 🏙️ Supporting smart city planning

---

## 🎯 Objective

* Simulate real-time traffic data
* Process streaming data using PySpark
* Detect congestion levels dynamically
* Visualize results using Streamlit dashboard

---

## 🧠 Tech Stack

* Python
* PySpark (Apache Spark)
* Streamlit
* Pandas
* Plotly Express
* Pyngrok

---

## 🔁 Project Architecture

Data Generation → Spark Streaming → Processing → Storage → Dashboard → Visualization → Ngrok

---

## ⚙️ Workflow

### 1️⃣ Data Generation

* Generates traffic data continuously
* Includes road, vehicle count, speed, timestamp, location

### 2️⃣ Spark Streaming

* Reads JSON data
* Processes in real time

### 3️⃣ Congestion Detection

* 🔴 HIGH → vehicle_count > 70 AND avg_speed < 30
* 🟠 MEDIUM → vehicle_count > 40
* 🟢 LOW → otherwise

### 4️⃣ Data Storage

* Stored in CSV files
* Updates every 5 seconds

### 5️⃣ Dashboard & Visualization

* Bar chart → congestion levels
* Line chart → trends
* Map → location insights

---

## ▶️ Run Project

```bash
pip install pyspark streamlit pandas pyngrok plotly

python data_generator.py
python spark_streaming.py
streamlit run app.py
```

