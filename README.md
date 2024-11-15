# Car Purchase Prediction

This project uses machine learning to predict whether a customer is likely to purchase a car based on their age and salary. The model is built using machine learning techniques and integrated with Flask for real-time prediction. This project offers valuable insights to automotive dealerships and businesses looking to analyze customer behavior.

## Table of Contents
- [Project Overview](#project-overview)
- [Technologies Used](#technologies-used)
- [Usage](#usage)
- [Modeling Approach](#modeling-approach)
- [Screenshots](#screenshots)

## Project Overview
The **Car Purchase Prediction** project uses a pre-trained machine learning model (K-Nearest Neighbors) to predict whether a customer will buy a car based on their **age** and **salary**. The project is designed to demonstrate how machine learning can be used to make predictions, with Flask providing a simple web interface to interact with the model.

## Technologies Used
- **Python 3.x**: Programming language used for model development and app logic.
- **Flask**: Web framework to serve the machine learning model through an interactive web interface.
- **scikit-learn**: For training and using the machine learning model.
- **joblib**: For saving and loading the trained model.
- **NumPy**: For handling numerical data and arrays.
- **HTML/CSS**: For the frontend user interface.

## Usage

### Running the Application
To start the Flask application, run the following command:
```bash
python app.py
```

The app will start running on `http://127.0.0.1:5000/` by default. Open the URL in your browser to interact with the app.

### How the Application Works
1. **Input Age and Salary**: The user is prompted to enter their age and estimated salary on the home page.
2. **Prediction**: After entering the data, the user clicks the **Predict** button. The app processes the input and displays the result on the result page.
3. **Result**: The model predicts whether the customer is likely to purchase a car or not based on the input values.

## Modeling Approach

1. **Data Collection**: The dataset consists of customer demographic data, including age, salary, and previous purchase history (if available).
   
2. **Preprocessing**:
   - Missing values were handled.
   - Categorical features were encoded (if applicable).
   - The data was normalized using a **scaler** to prepare it for model input.

3. **Model Development**:
   - **K-Nearest Neighbors (KNN)** was chosen as the machine learning model for classification. Other models like Logistic Regression or Random Forest could also be used for comparison.
   
4. **Training the Model**:
   - The model was trained on historical customer data to learn patterns that correlate age and salary with car purchase behavior.

5. **Model Evaluation**:
   - Accuracy, precision, and recall were evaluated to determine how well the model predicts customer interest.

6. **Saving the Model**:
   - The trained model and the scaler were saved using `joblib` for later use in the Flask app.

## Screenshots

### Home Page
![Home Page](https://github.com/user-attachments/assets/e4436d19-44c4-430d-90f8-1f6103755ebd)
![Home Page](https://github.com/user-attachments/assets/a4f8c16d-c118-4540-93cb-6868f031a131)

### Result Page
![Result Page](https://github.com/user-attachments/assets/65df6f04-e24e-4608-85fa-99604cc8f75d)
