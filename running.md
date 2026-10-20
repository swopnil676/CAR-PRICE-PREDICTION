# Running the Car Price Prediction Project

This guide explains how to start the FastAPI backend and Streamlit frontend in two separate terminals.

## 1. Start the FastAPI Backend

Open **Terminal 1** in VS Code.

Change to the backend project root:

```powershell
cd "A:\CODING\COMPLETE AGI ENGINEERING\Fast API (backend)\car-price-api\app"
```

Start the backend:

```powershell
python -m uvicorn main:app --reload
```

- **Backend URL:** http://127.0.0.1:8000
- **API documentation:** http://127.0.0.1:8000/docs

Keep this terminal running.

## 2. Start the Streamlit Frontend

Open **Terminal 2** in VS Code. Keep the backend terminal running.

Change to the frontend directory:

```powershell
cd "A:\CODING\COMPLETE AGI ENGINEERING\Fast API (backend)\car-price-api"
```

Start Streamlit:

```powershell
python -m streamlit run streamlit_app.py
```

Streamlit usually opens at:

- **Frontend URL:** http://localhost:8501

## Important Notes

- Start FastAPI first, then start Streamlit.
- Keep both terminals running while using the application.
- Make sure the frontend sends requests to the correct backend URL: `http://127.0.0.1:8000`.
- If your frontend folder is stored in a different location, update the directory path in the command.
- Ensure Streamlit is installed in the active Python environment. If needed, run `python -m pip install streamlit`.