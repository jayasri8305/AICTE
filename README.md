

# EV Adoption Forecasting for Washington State Counties

## Project Overview  
This project develops a predictive model and interactive dashboard to forecast electric vehicle (EV) adoption trends by county in Washington State. Using historical monthly EV registration data, we build a regression model to predict EV growth over the next 3 years. The resulting forecasts can aid policymakers and planners in infrastructure development, especially charging station deployment.

## Features  
- Data preprocessing with lag features, rolling means, and growth slopes  
- Random Forest regression model with hyperparameter tuning for accurate forecasting  
- Interactive Streamlit app for visualizing county-level EV adoption trends  
- Multi-county comparison capabilities for side-by-side growth analysis  
- Visualizations of historical and forecasted cumulative EV count  

## Installation  
1. Clone the repository:  
   ```bash
   git clone https://github.com/yourusername/ev-adoption-forecast.git
   cd ev-adoption-forecast
   ```
2. Create and activate a virtual environment (optional but recommended):  
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```
3. Install required packages:  
   ```bash
   pip install -r requirements.txt
   ```
4. Download the dataset from [Kaggle - Electric Vehicle Population Size 2024](https://www.kaggle.com/datasets/sahirmaharajj/electric-vehicle-population-size-2024/data) and place `Electric_Vehicle_Population_By_County.csv` in the project folder.

## Usage  
1. Preprocess data and train model (optional, if you want to retrain):  
   Run the Jupyter notebook or Python script for preprocessing and training.  
2. Run the Streamlit app:  
   ```bash
   streamlit run app.py
   ```
3. Open the URL provided by Streamlit in your browser to interact with the EV adoption forecast tool.

## Project Structure  
- `app.py`: Streamlit application code for interactive forecast visualization  
- `preprocessed_ev_data.csv`: Processed dataset with engineered features  
- `forecasting_ev_model.pkl`: Trained Random Forest model serialized with joblib  
- `ev-car-factory.jpg`: Image used in Streamlit app UI  
- Jupyter notebooks / scripts for data preprocessing and model training  

## Dependencies  
- Python 3.10 or newer  
- streamlit  
- pandas  
- numpy  
- scikit-learn  
- matplotlib  
- joblib  

See `requirements.txt` for full list.

## Results  
The model forecasts electric vehicle adoption trends with strong predictive performance (R² score and error metrics included in project notebook). The interactive app displays cumulative EV growth per county with forecasted trends for the next 3 years, enabling comparative analysis across multiple counties.


