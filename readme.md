<h1>Real Estate Price Predictor</h1>
Description
This project is a machine learning model that predicts real estate prices in Bengaluru based on various features such as location, square footage, number of bedrooms (BHK), and bathrooms. It preprocesses the dataset, removes anomalies, and applies different regression models to make accurate predictions. The best-performing model is saved for future use.
Prerequisites
Before running the code, you need to set up a virtual environment and install the required dependencies to ensure a clean and controlled Python environment.
Setting Up the Virtual Environment
1. Open a terminal or command prompt.
2. Navigate to the project directory where real_state_price_predictor.ipynb is located.
3. Run the following command to create a virtual environment:
4. python -m venv venv
5. Activate the virtual environment:
* Windows:
* venv\Scripts\activate
* macOS/Linux:
* source venv/bin/activate
Installing Dependencies
Once the virtual environment is activated, install the required dependencies using the following command:
pip install -r requirements.txt
If requirements.txt is not available, manually install the following libraries:
pip install numpy pandas matplotlib scikit-learn pickle-mixin jupyter
Running the Project
1. Ensure the virtual environment is activated.
2. Launch Jupyter Notebook by running:
3. jupyter notebook
4. Open real_state_price_predictor.ipynb and execute the cells in order.
Features Implemented
* Data Preprocessing:
* Removing unnecessary columns.
* Handling missing values.
* Standardizing numerical data.
* Feature Engineering:
* Creating new features such as bhk and price_per_sqft.
* Encoding categorical variables.
* Outlier Detection & Removal:
* Removing extreme property price variations.
* Handling anomalies in total_sqft and bathroom count.
* Model Selection & Training:
* Training models using Linear Regression, Lasso Regression, and Decision Tree Regressor.
* Hyperparameter tuning using GridSearchCV.
* Cross-validation for improved accuracy.
* Price Prediction Function:
* Allows users to input property details and get a price estimate.
Output
* The trained model is saved as banglore_home_prices_model.pickle.
* Feature columns are stored in columns.json.
* The predict_price function can be used to estimate property prices based on input parameters such as location, size, and number of rooms.
Libraries Used
* numpy - For numerical computations.
* pandas - For data manipulation.
* matplotlib - For data visualization.
* scikit-learn - For machine learning models and preprocessing.
* pickle - For saving and loading the trained model.
* json - For handling feature column data.
* jupyter - For running the notebook interactively.

