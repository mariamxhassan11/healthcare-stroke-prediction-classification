# Stroke Prediction

End-to-end clinical risk classification pipeline predicting patient stroke probability from demographic and health indicators.

## Project Structure

```text
01_Stroke_Prediction/
├── stroke_prediction_data.csv
├── stroke_prediction_pipeline.ipynb
├── app.py
├── best_model.pkl
├── model_metadata.json
├── requirements.txt
└── README.md
```

## Dataset & Features

- **Dataset File:** `stroke_prediction_data.csv`
- **Task Type:** `Classification`
- **Target Variable:** `stroke`
- **Numerical Features (5):** `age, hypertension, heart_disease, avg_glucose_level, bmi`
- **Categorical Features (5):** `gender, ever_married, work_type, Residence_type, smoking_status`

## Model Evaluation Summary

- **Selected Best Model:** `LogisticRegression`

| Metric | Score |
| :--- | :--- |
| `accuracy` | `0.9444` |
| `f1_score` | `0.9153` |
| `roc_auc` | `0.9859` |

## Quickstart & Deployment

1. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
2. Run the Streamlit web application:
   ```bash
   streamlit run app.py
   ```
