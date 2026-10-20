# 🚗 Car Price Prediction

A machine learning project that predicts the selling price of a used car using a **Random Forest Regressor**. The project provides a FastAPI backend for predictions and a Streamlit frontend for user interaction.

## ✨ Features

- Predict used car selling prices using a trained Random Forest model.
- FastAPI backend with a REST API.
- Streamlit frontend for entering car details and viewing predictions.
- Input validation using Pydantic.
- Interactive API documentation with Swagger UI.
- Model inference using Pandas and Scikit-learn.

## 🛠️ Technologies Used

- **Language:** Python
- **Machine Learning:** Scikit-learn, Random Forest Regressor
- **Backend:** FastAPI, Uvicorn
- **Frontend:** Streamlit
- **Data Processing:** Pandas, NumPy
- **Model Storage:** Joblib

## 📁 Project Structure

```text
CAR-PRICE-PREDICTION/
├── app/
│   ├── main.py
│   ├── model.py
│   └── schema.py
├── streamlit_app.py
├── models/
│   ├── random_forest_model.pkl
│   └── feature_column.pkl
├── requirements.txt
├── README.md
└── train.py
```

*Adjust the structure above to match your actual repository and the locations of your model files.*

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone https://github.com/swopnil676/CAR-PRICE-PREDICTION
cd car-price-api
```

Replace `https://github.com/swopnil676/CAR-PRICE-PREDICTION` with your actual GitHub repository URL.

### 2. Create and activate a virtual environment

On Windows PowerShell:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

### 3. Install dependencies

```powershell
python -m pip install -r requirements.txt
```

## ▶️ How to Run the Project

Run the backend and frontend in **two separate terminals**.

### 1. Start the FastAPI Backend

Open Terminal 1 in VS Code and navigate to the backend project root, the directory containing the `app` folder.

```powershell
python -m uvicorn app.main:app --reload
```

Backend URL: http://127.0.0.1:8000

API documentation: http://127.0.0.1:8000/docs

Keep this terminal running.

### 2. Start the Streamlit Frontend

Open Terminal 2 in VS Code and navigate to the frontend directory:

```powershell
cd frontend
```

Start the frontend:

```powershell
python -m streamlit run streamlit_app.py
```

Frontend URL: http://localhost:8501

Keep both terminals running while using the application.

> Run the commands from the correct directories. If your frontend is outside the backend project folder, navigate to its actual location instead.

## 🔮 Future Improvements

- Improve prediction accuracy through model evaluation and feature engineering.
- Add more visualizations and model performance metrics.
- Deploy the frontend and backend for public access.
- Add automated tests and improved error handling.

## 👨‍💻 Author

**Swopnil Biswas**

- GitHub: [swopnil676](https://github.com/swopnil676)

---

⭐ If you find this project useful, consider giving the repository a star!
