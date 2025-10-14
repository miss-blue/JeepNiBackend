# JeepNi Backend System

## Core Files

### Main Application Files
- `app.py` - Main Flask application setup with database configuration, CORS setup, and core middleware
- `main.py` - Application entry point and server startup
- `routes.py` - API endpoint definitions and route handlers for the web interface
- `models.py` - SQLAlchemy database models and schema definitions

### Machine Learning Components
- `ml_pipeline.py` - XGBoost-based passenger forecasting model implementation 
- `data_generator.py` - Synthetic data generation for model training
- `scheduler.py` - Automated prediction generation and scheduling system
- `passenger_demand_data.csv` - Generated dataset for passenger demand predictions

### External Services
- `firebase_service.py` - Firebase integration for notifications and user management

## Directories

### /data
- Storage directory for model data and cached predictions

### /instance
- Flask instance-specific files and configuration
- Contains database files and local settings

### /notebooks
- `data_analysis.ipynb` - Data exploration and statistical analysis
- `model_development.ipynb` - Model training and evaluation experiments
- `passenger_forecasting_analysis.ipynb` - Passenger demand pattern analysis

## Utility Files
- `run_jupyter.py` - Helper script to launch Jupyter notebooks
- `.gitignore` - Git version control ignore patterns

## Key Features

1. **Passenger Demand Forecasting**
   - Machine learning pipeline for predicting passenger volumes
   - Automated daily predictions for each stop
   - Model performance monitoring and retraining

2. **Real-time Notifications**
   - Firebase integration for push notifications
   - SMS notifications via external API

3. **Data Management**
   - Synthetic data generation for model training
   - Historical prediction storage
   - Stop and user data management

4. **API Endpoints**
   - REST API for predictions and user management
   - Admin dashboard interface
   - Rate-limited SMS gateway