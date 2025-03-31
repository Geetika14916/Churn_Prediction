# Customer Churn Prediction

This project is a machine learning application that predicts customer churn using a deep learning model built with TensorFlow and scikit-learn. The model takes in customer attributes and determines the likelihood of churn.

## Features
- **Uses a trained TensorFlow model** (`model.h5`) to make predictions.
- **Preprocesses input data** with `scikit-learn` encoders and scalers.
- **Streamlit web interface** for easy user interaction.
- **Notebook-based prediction (`prediction.ipynb`)** for testing the model.

## Installation

### 1️⃣ Clone the Repository
```bash
git clone <repository-url>
cd <project-folder>
```

### 2️⃣ Set Up a Virtual Environment
```bash
python -m venv venv
source venv/bin/activate  # On Mac/Linux
venv\Scripts\activate    # On Windows
```

### 3️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

## Running the Project

### Streamlit App
Run the Streamlit web application:
```bash
streamlit run app.py
```

### Jupyter Notebook
Run the `prediction.ipynb` notebook to test the model with sample inputs.

## Files Overview
- `app.py` → Streamlit web app for user interaction.
- `prediction.ipynb` → Jupyter Notebook for testing the model.
- `model.h5` → Pretrained TensorFlow model.
- `label_encoder_gender.pkl` → Label encoder for gender feature.
- `onehot_encoder_geo.pkl` → One-hot encoder for geography feature.
- `sscaler.pkl` → Standard scaler for numerical features.

## Dependencies
Ensure you have the following installed:
```txt
tensorflow==2.17.1
scikit-learn>=1.2
pandas
numpy
streamlit
```

To update TensorFlow and other dependencies:
```bash
pip install --upgrade tensorflow scikit-learn pandas numpy streamlit
```

## Troubleshooting
- **`model.h5` not loading?** Try:
  ```python
  model = tf.keras.models.load_model("model.h5", compile=False)
  ```
- **OneHotEncoder warning?** Ensure that feature names are correctly handled.

## Future Improvements
- Add a retraining script to update the model.
- Deploy the application using a cloud service (e.g., AWS, Google Cloud).

---
### ✨ Developed with Machine Learning & Streamlit 🚀

