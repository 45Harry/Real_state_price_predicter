Real Estate Price Predictor
Description

This project is a machine learning model that predicts real estate prices in Bengaluru based on various features such as location, square footage, number of bedrooms (BHK), and bathrooms. The process involves preprocessing the dataset, removing anomalies, and applying different regression models to make accurate predictions. The best-performing model is then saved for future use.
Prerequisites

Before running the code, you need to set up a virtual environment and install the required dependencies to ensure a clean and controlled Python environment.
Setting Up the Virtual Environment

    Open a terminal or command prompt.
    Navigate to the project directory where real_state_price_predictor.ipynb is located.
    Run the following command to create a virtual environment:

python -m venv venv

Activate the virtual environment:

    Windows:

        venv\Scripts\activate

macOS/Linux:

        source venv/bin/activate

Installing Dependencies

Once the virtual environment is activated, install the required dependencies using the following command:

pip install -r requirements.txt

If requirements.txt is not available, manually install the following libraries:

pip install numpy pandas matplotlib scikit-learn pickle-mixin jupyter

Running the Project

    Ensure the virtual environment is activated.
    Launch Jupyter Notebook by running:

    jupyter notebook

    Open real_state_price_predictor.ipynb and execute the cells in order.

Features Implemented
1. Data Preprocessing:

    Removing unnecessary columns.
    Handling missing values.
    Standardizing numerical data.

2. Feature Engineering:

    Creating new features such as bhk (number of bedrooms) and price_per_sqft.
    Encoding categorical variables.

3. Outlier Detection & Removal:

    Removing extreme property price variations.
    Handling anomalies in total_sqft and bathroom count.

4. Model Selection & Training:

    Training models using:
        Linear Regression
        Lasso Regression
        Decision Tree Regressor
    Hyperparameter tuning using GridSearchCV.
    Cross-validation for improved accuracy.

5. Price Prediction Function:

    Allows users to input property details and get a price estimate.

Output

    The trained model is saved as banglore_home_prices_model.pickle.
    Feature columns are stored in columns.json.
    The predict_price function can be used to estimate property prices based on input parameters such as location, size, and number of rooms.

Libraries Used

    numpy: For numerical computations.
    pandas: For data manipulation.
    matplotlib: For data visualization.
    scikit-learn: For machine learning models and preprocessing.
    pickle: For saving and loading the trained model.
    json: For handling feature column data.
    jupyter: For running the notebook interactively.
