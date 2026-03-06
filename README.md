# End-to-End ML Deployment with CatBoost 

## Overview  
This project demonstrates a complete machine learning workflow—from data ingestion to model deployment—in Python. Leveraging CatBoost for structured data modeling, the trained model is served via a Flask web application for real-time inference.

<img src="https://github.com/Harry160820/End-to-End-ML-Deployment-with-CatBoost/edit/main/README.md#:~:text=to%2Dend%2DML.-,png,-README.md" alt="Alt text" width="500">

## Tech Stack  
- **Data Processing & Modeling**: Python, pandas, NumPy, CatBoost  
- **Web App**: Flask (app.py)  
- **Project Structure**:
  - `src/`: Data preprocessing & model training  
  - `notebook/`: Jupyter notebook for EDA, feature engineering & tuning  
  - `app.py`: Flask API for model predictions  
- **Dependencies**: Listed in `requirements.txt`, managed via `setup.py`

## Features  
- Preprocess raw data, engineer features, train & validate a CatBoost model  
- Save trained model and load using `joblib` within Flask  
- Build REST API endpoint that accepts input JSON and returns predictions  

## Results  
- Achieved **88.04% accuracy** 
- API supports **100+ requests per minute** at <50ms latency (benchmark locally)  

## Usage  
1. Clone the repo  
2. `pip install -r requirements.txt`  
3. Run `main.py` to preprocess, train & save model  
4. Start server: `python app.py`  
5. Send POST requests to `/predict` with JSON input  

## Next Steps  
- Integrate CI/CD with GitHub Actions  
- Dockerize the app for scalable deployment  
- Add authentication, logging, and visualization in Flask UI

## Contributing  
Feel free to open issues or PRs. For major changes, kindly create an issue to discuss first.

---

