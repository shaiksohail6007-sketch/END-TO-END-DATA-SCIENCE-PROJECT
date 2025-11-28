# END-TO-END-DATA-SCIENCE-PROJECT

*COMPANY: CODTECH IT SOLUTION

*NAME: SHAIK SOHAIL

*INTERN ID: CT04DR1947

*DOMAIN: DATA SCIENCE

*DURATION: 4 WEEKS

*MENTOR: NEELA SANTHOSH

##End-to-End Data Science Project.
The objective of this task is to demonstrate the full life cycle of a data science solution — beginning from data collection, preprocessing, model building, all the way to deploying a functional API using Flask. This task integrates multiple aspects of the modern data science workflow and simulates a realistic scenario followed in industry projects.

End-to-end data science projects are highly valuable because they show a complete transition from raw data to a fully deployed ML-powered service. Such systems are widely used in machine learning applications across business, technology, automation, and cloud environments. This task shows your ability to work not just on the model, but also on deployment, delivering a real-world solution.

Task Objective
To collect or create a dataset for a specific business problem.
To clean and preprocess the data using Python.
To train a machine learning model.
To save the model using serialization (pickle).
To build a deployment-ready API using Flask or FastAPI.
To test predictions through HTTP requests.
To simulate how a real ML model is served in production.

Tools & Technologies Used
Programming Language:
Python 3.10

Libraries Used:
Pandas → Data loading, cleaning, manipulation
NumPy → Numerical processing
Scikit-learn → Model training, scaling, regression
Flask → API development and deployment
Pickle → Saving trained ML models
Requests / curl → API testing

Platform / Environment:
Visual Studio Code (VS Code) for coding
Windows OS
Virtual Environment (tfenv) used for clean dependency management
Browser for API testing (Postman / Invoke-RestMethod)
Version Control:
Git + GitHub

Where This Project Can Be Applied (Real-World Use Cases)
End-to-end ML systems like this are widely used in:
1. Real Estate Price Prediction Platforms
Websites like MagicBricks and Zillow use ML models to predict house prices instantly.

2. Financial Loan Prediction Systems
Banks use deployed ML APIs to determine loan approval chances.

3. Ecommerce Recommendation & Analytics
Predictive APIs help suggest products and pricing strategies.

4. Healthcare Diagnosis & Automation
Backend ML APIs classify diseases or predict health risks.

5. Manufacturing Quality Control
Models predict equipment failures or product defects.

6. Enterprise Reporting Automation
Organizations automate weekly predictions (sales, demand, stock).

7. Cloud-Based ML Services
Companies deploy ML models on AWS Lambda, Azure ML, Heroku, etc.

This task mimics exactly how companies deploy ML models in real applications.

Project Structure
├── housing.csv                 # Dataset
├── training.py                 # Trains the ML model
├── model.pkl                   # Saved trained model
├── scaler.pkl                  # Saved data scaler
├── app.py                      # Flask API app
├── README.md                   # Project documentation
└── tfenv/                      # Python virtual environment

Data Collection & Preprocessing
The dataset used (housing.csv) includes features such as:
bedrooms
bathrooms
area (sq. ft.)
age of house
price (target variable)

Preprocessing Steps:
Handling missing values
Cleaning numerical data
Scaling features using StandardScaler
Splitting dataset into train/test sets
Creating regression model
This ensures the data is model-ready and avoids bias or imbalance.

Model Training
A Linear Regression model is trained using Scikit-learn.
The steps include:
Fit the scaled features
Train the model
Evaluate using R² score
Save model + scaler using pickle

Example output:

Model R²: 0.74
model.pkl saved
scaler.pkl saved

Model Deployment (Flask API)

The app.py file creates a simple API:
/ → Home route
/predict → Accepts JSON input and returns predicted house price

Example API request:
{
  "bedrooms": 3,
  "bathrooms": 2,
  "area": 1500,
  "age": 10
}


API Response:

{
  "predicted_price": 108383.23
}

This demonstrates a fully deployed ML model accessible over HTTP.

Testing the API
Using PowerShell:
Invoke-RestMethod -Uri "http://127.0.0.1:5000/predict" -Method Post -Body '{"bedrooms":3,"bathrooms":2,"area":1500,"age":10}' -ContentType "application/json"

Confirms model is served correctly
Produces real prediction output

Conclusion
This end-to-end data science project demonstrates how raw data can be transformed into a fully functional machine learning service. The project covers data preprocessing, model building, saving the trained model, and deploying it using a Flask API. This mirrors the real process used by data scientists, ML engineers, and AI teams in production systems.

The ability to deploy a model is a crucial skill because real-world ML is only useful when it is integrated into applications. This task showcases full-stack data science skills — from data to deployment — making it a valuable and practical project for your internship portfolio.

#OUTPUT

<img width="960" height="1020" alt="Image" src="https://github.com/user-attachments/assets/12c75dc2-2a8d-40be-9fae-957cea5b6ae7" />

<img width="957" height="1032" alt="Image" src="https://github.com/user-attachments/assets/5cd32a35-a436-4100-91f7-a03fb3bc2351" />
