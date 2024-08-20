# Car-Prices-Predicting

The document you uploaded outlines the process of predicting used car prices using machine learning techniques. Here's a summary of the key steps and concepts:

1. **Import Libraries**: The document starts by importing necessary libraries for data manipulation, visualization, and machine learning, such as `numpy`, `pandas`, `matplotlib`, `seaborn`, and `sklearn`.

2. **Data Loading and Exploration**:
   - The dataset is loaded using `pandas`. It includes various features like car name, location, year, kilometers driven, fuel type, transmission, owner type, mileage, engine capacity, power, and seats.
   - The dataset is split into training and test sets to evaluate the models' performance.

3. **Exploratory Data Analysis (EDA)**:
   - The index column is removed as it's not necessary for the analysis.
   - The car manufacturer is extracted from the car name to simplify the dataset.
   - Unnecessary columns like `Name` and `Location` are dropped, as they don't contribute to predicting car prices.
   - The `Year` column is transformed to represent the age of the car.
   - Categorical columns (`Fuel_Type`, `Transmission`, `Owner_Type`) are prepared for modeling by converting them into dummy variables.
   - Numerical features like `Kilometers_Driven`, `Mileage`, `Engine`, and `Power` are cleaned and scaled to standardize the data.

4. **Data Processing**:
   - Dummy variables are created for categorical features.
   - Missing columns in the test data are filled with zeros to match the training data structure.
   - The data is then scaled using `StandardScaler` to normalize the feature values.

5. **Model Training and Prediction**:
   - Two models are trained: a Linear Regression model and a Random Forest model.
   - The performance of these models is evaluated using the R² score.
   - The Random Forest model outperformed Linear Regression, achieving an R² score of 0.88.

In summary, the document describes the steps to clean, process, and model a dataset for predicting used car prices, demonstrating that the Random Forest model provides better predictions compared to Linear Regression.
