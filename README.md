# 🔧 Cooler Failure Prediction (Hydraulic System Monitoring)

This repository contains a complete machine learning pipeline for predicting industrial **cooler failures** using sensor data from a hydraulic system. It includes:

- 📊 A well-documented Jupyter notebook for data preprocessing, feature engineering, model training, and evaluation
- 📈 A visual prediction chart comparing real vs. predicted failures
- 🧠 A trained Random Forest model based on selected features
- 🖥️ An interactive **Streamlit dashboard** for viewing model performance
- 📁 A downloadable dataset (hosted on Google Drive)

---

## 📂 Folder Structure

```
├── SRC/                          # Contains Jupyter notebook (.ipynb)
│   └── cooler_model_clean_final.ipynb
├── cooler_dashboard.py          # Streamlit dashboard application
├── evaluation.csv               # Prediction results with actual vs. predicted labels
├── prediction_chart.png         # Smoothed failure probability chart
└── DATA/                        # (Optional placeholder, data is external)
```

---

## 📥 Download the Dataset

The dataset used in this project can be downloaded from the link below:

🔗 **[Download Sensor Dataset (Google Drive)](https://drive.google.com/file/d/1kXLs2nPt_CG6r7ywiyD1X4cTmp_bdWGP/view?usp=drive_link)**

After downloading:
1. Extract the zip file.
2. Place the `.txt` files (e.g., TS1.txt, PS5.txt, profile.txt...) in a folder named `hydrolic`.
3. Update the `base_path` in the notebook if your local path is different:
   ```python
   base_path = "E:/automation/IOT/hydrolic/"
   ```

---

## 🚀 How to Run

### 1. Run the Model Notebook

Open the notebook:

```
SRC/cooler_model_clean_final.ipynb
```

Run it cell by cell. It will:
- Load and process data
- Engineer features
- Train a Random Forest classifier
- Evaluate and visualize model performance
- Save `evaluation.csv`, `prediction_chart.png`, and `dashboard.html`

---

### 2. Launch the Streamlit Dashboard

In terminal or Anaconda Prompt:

```bash
cd E:/automation/IOT/
streamlit run cooler_dashboard.py
```

This launches a visual web dashboard at:  
📍 http://localhost:8501

---

## 📊 Model Performance

| Metric           | Value |
|------------------|-------|
| Accuracy         | 100%  |
| Precision (Fail) | 100%  |
| Recall (Fail)    | 100%  |
| TP / TN / FP / FN| 288 / 148 / 0 / 0 |

The prediction chart and evaluation table are stored in:

- `prediction_chart.png`
- `evaluation.csv`

---

## ✨ Highlights

- ✅ Simple and clean pipeline
- ✅ Intuitive visualizations
- ✅ Modular code and reproducible results
- ✅ Easy to deploy or integrate with SCADA/IoT dashboards

---

## 👨‍💻 Author

Prepared by **Vahid Shakeri**  
For project inquiries: [LinkedIn](https://www.linkedin.com/in/vahid-shakeri-194262183/)

---

## 📄 License

This project is provided for educational and demonstration purposes. Use it freely with attribution.