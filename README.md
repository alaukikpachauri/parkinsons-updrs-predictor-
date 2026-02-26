# 🧠 Parkinson's UPDRS Predictor

A Machine Learning model that predicts **Total UPDRS** and **Motor UPDRS** scores for Parkinson's disease patients based on biomedical voice measurements.

---

## 📌 About the Project

This project uses the **Oxford Parkinson's Disease Telemonitoring Dataset** to build a Multi-Output Random Forest Regressor that predicts disease severity scores (UPDRS) from voice features. A **Gradio web interface** is provided for easy interaction with the model.

---

## 📊 Dataset

- **Source:** [Kaggle - Parkinson Dataset by leilahasan](https://www.kaggle.com/datasets/leilahasan/parkinson-dataset)
- **Records:** 5,875 voice recordings from 42 patients with early-stage Parkinson's disease
- **Target Variables:** `total_UPDRS`, `motor_UPDRS`

### Key Features Used:
| Feature | Description |
|---|---|
| `age` | Age of the patient |
| `PPE` | Pitch Period Entropy |
| `RPDE` | Recurrence Period Density Entropy |
| `Shimmer:APQ11` | Shimmer measure |
| `Shimmer(dB)` | Shimmer in decibels |
| `Shimmer` | Local shimmer |
| `Shimmer:APQ5` | Shimmer APQ5 measure |

---

## 🛠️ Tech Stack

- Python 3.x
- Pandas, NumPy
- Scikit-learn
- Gradio
- KaggleHub

---

## 🚀 How to Run

### 1. Clone the repository
```bash
git clone https://github.com/your-username/parkinsons-updrs-predictor.git
cd parkinsons-updrs-predictor
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Run the notebook
Open `ugh__4_.ipynb` in Jupyter Notebook or Google Colab and run all cells.

> **Note:** The dataset is downloaded automatically via `kagglehub`. Make sure you have a Kaggle account and your API key configured.

---

## 📈 Model Performance

| Metric | Training | Test |
|---|---|---|
| MAE | 1.11 | 3.11 |
| MSE | 2.74 | 20.55 |
| R² Score | 0.969 | 0.750 |

---

## 🖥️ Gradio Interface

The project includes an interactive web UI built with Gradio where you can input voice features and get predicted UPDRS scores in real time.

![Gradio UI](https://www.gradio.app/assets/img/header-image.jpg)

---

## 📁 Project Structure

```
parkinsons-updrs-predictor/
│
├── ugh__4_.ipynb        # Main notebook
├── requirements.txt     # Python dependencies
├── README.md            # Project documentation
└── .gitignore           # Git ignore rules
```

---

## 🙋 Author

Made with ❤️ for learning and academic purposes.
