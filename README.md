#  Aircraft Engine RUL Prediction System

##  Overview

This project predicts the **Remaining Useful Life (RUL)** of aircraft engines using Machine Learning, Deep Learning, Graph Neural Networks, and a Hybrid AI model. It also provides risk analysis, visualization, and AI-based maintenance suggestions.

---

##  Features

* User Login & Registration (Flask + SQLite)
* Multiple Models:

  * Random Forest
  * CNN
  * LSTM
  * GNN
  * Hybrid Model (LSTM + GNN + NLP)
* RUL Prediction
* Risk Level Detection (High / Moderate / Low)
* Graph Visualization
* AI-based Maintenance Explanation

---

##  Models Used

* Random Forest (Baseline ML)
* CNN (Feature extraction)
* LSTM (Time-series learning)
* GNN (Sensor relationship modeling)
* Hybrid Model (Best performance)

---

##  Project Structure

```
project/
│
├── app.py
├── base.py
├── gnn.py
├── hybrid.py
│
├── templates/
├── static/
│
├── requirements.txt
└── README.md
```

---

##  Installation

```bash
git clone https://github.com/your-username/rul-prediction.git
cd rul-prediction
pip install -r requirements.txt
```

---

## ▶️ Run Application

```bash
python app.py
```

Open in browser:

```
http://127.0.0.1:5000/
```

---

##  Model Training

Train all models separately:

```bash
python train_model.py
python train_gnn.py
python train_hybrid.py
```

---

##  Output

* Predicted RUL
* Actual RUL
* Accuracy %
* Risk Level (High / Moderate / Low)
* Graphs:

  * Prediction vs Actual
  * Sensor Trends
  * Model Comparison

---

##  Dataset

NASA Turbofan Engine Dataset (CMAPSS)

---

##  AI Explanation

Uses Groq API (LLaMA model) to generate:

* Maintenance suggestions
* Risk explanation
* Failure reasoning

---

##  Technologies

* Python
* Flask
* PyTorch
* TensorFlow / Keras
* Scikit-learn
* Torch Geometric
* Sentence Transformers
* Matplotlib

---

##  Security Note

Do NOT upload your API key.

Replace:

```python
client = Groq(api_key="YOUR_KEY")
```

With:

```python
import os
client = Groq(api_key=os.getenv("GROQ_API_KEY"))
```

---

## Author

Champakam N

---

##  License

For academic and research use only.

