# Student Performance Prediction (End-to-End ML Pipeline)

This project implements a production-ready Machine Learning pipeline to predict student math scores based on demographic and school-related features. It is built with a modular architecture to ensure scalability, maintainability, and ease of deployment.

---

## 🏗 Project Structure

The codebase is organized into logical components to handle the full ML lifecycle:

* **`src/components/`**: 
    * `data_ingestion.py`: Handles data loading from sources and performs train-test splits.
    * `data_transformation.py`: Implements a preprocessing pipeline using `ColumnTransformer` for numerical scaling and categorical encoding.
    * `model_trainer.py`: Evaluates multiple models (Random Forest, XGBoost, CatBoost, etc.) and performs hyperparameter tuning.
* **`src/pipeline/`**:
    * `predict_pipeline.py`: A dedicated script for loading the serialized model and preprocessor to generate real-time predictions.
* **`app.py`**: A Flask web application providing a user interface for data input and prediction.
* **`artifacts/`**: Directory where the trained `model.pkl` and `preprocessor.pkl` are stored.

---

## 🚀 Getting Started

### 1. Installation
Clone the repository and install the dependencies:
```bash
git clone [https://github.com/dhawalpanchal1997/mlproject.git](https://github.com/dhawalpanchal1997/mlproject.git)
cd mlproject
pip install -r requirement.txt
