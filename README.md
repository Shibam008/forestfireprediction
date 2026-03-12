# 🔥 Fire Weather Index (FWI) Prediction Web Application

## 📌 Project Overview

This project is a **Machine Learning web application** that predicts the **Fire Weather Index (FWI)** using meteorological and environmental parameters.
The model is trained using the **Algerian Forest Fires Dataset**, which contains weather observations and fire occurrence records collected from two regions of Algeria.

The goal of this project is to demonstrate the **end-to-end Machine Learning workflow**, including:

* Data Cleaning
* Exploratory Data Analysis (EDA)
* Feature Engineering
* Model Training
* Model Evaluation
* Deployment using **Flask Web Framework**

Users can input environmental parameters through a **web interface**, and the trained machine learning model predicts the **Fire Weather Index value**, which indicates the potential risk of forest fires.

---

# 🌍 What is Fire Weather Index (FWI)?

The **Fire Weather Index (FWI)** is a numerical rating system used worldwide to estimate the **intensity of forest fires** based on weather conditions.

It combines multiple environmental factors such as:

* Temperature
* Humidity
* Wind speed
* Rainfall
* Fuel moisture

A **higher FWI value indicates a higher probability and intensity of fire spread.**

Typical interpretation:

| FWI Value | Fire Risk |
| --------- | --------- |
| < 5       | Low       |
| 5 – 20    | Moderate  |
| > 20      | High      |

---

# 📊 Dataset

This project uses the **Algerian Forest Fires Dataset**.

Dataset characteristics:

* **244 observations**
* Collected from **Bejaia region** and **Sidi Bel-Abbes region**
* Weather and fire occurrence data

Features used in the model:

| Feature     | Description                |
| ----------- | -------------------------- |
| Temperature | Air temperature in Celsius |
| RH          | Relative Humidity (%)      |
| Ws          | Wind Speed (km/h)          |
| Rain        | Rainfall amount (mm)       |
| FFMC        | Fine Fuel Moisture Code    |
| DMC         | Duff Moisture Code         |
| ISI         | Initial Spread Index       |
| Classes     | Fire occurrence indicator  |
| Region      | Geographic region          |

Target Variable:

* **FWI (Fire Weather Index)**

---

# 🧠 Machine Learning Workflow

The project follows a standard **ML pipeline**:

### 1️⃣ Data Cleaning

* Handling missing values
* Removing inconsistent entries
* Converting categorical variables

### 2️⃣ Exploratory Data Analysis

* Distribution analysis
* Correlation analysis
* Outlier detection

### 3️⃣ Feature Engineering

* Encoding categorical features
* Scaling numerical features using **StandardScaler**

### 4️⃣ Model Training

Multiple regression models were explored:

* Linear Regression
* Ridge Regression
* Lasso Regression
* ElasticNet Regression

### 5️⃣ Model Evaluation

Models were evaluated using:

* **R² Score**
* **Mean Absolute Error**
* **Mean Squared Error**

The best performing model was selected for deployment.

---

# 🚀 Web Application

A simple **Flask-based web application** was built to allow users to interact with the trained model.

### User Input Parameters

Users provide the following environmental values:

* Temperature
* Relative Humidity
* Wind Speed
* Rainfall
* FFMC
* DMC
* ISI
* Classes
* Region

The application processes these inputs and returns the **predicted Fire Weather Index**.

---

# 🖥️ Project Structure

```
linear-regression-project
│
├── notebooks
│   ├── Data_cleaning_observation.ipynb
│   └── Regularizations_and_CrossValidation.ipynb
│
├── templates
│   └── home.html
│
├── application.py
├── requirements.txt
├── README.md
└── .gitignore
```

---

# ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/linear-regression-project.git
```

Navigate to the project directory:

```bash
cd linear-regression-project
```

Create a virtual environment:

```bash
python -m venv venv
```

Activate the environment:

Windows

```bash
venv\Scripts\activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

# ▶️ Running the Application

Run the Flask app:

```bash
python application.py
```

Open your browser and go to:

```
http://127.0.0.1:5000/
```

You will see the **FWI Prediction Interface** where you can enter weather parameters and obtain predictions.

---

# 📈 Example Workflow

1. Enter weather parameters in the form
2. Click **Predict**
3. The trained machine learning model processes the inputs
4. The predicted **Fire Weather Index value** is displayed

---

# 🧰 Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn
* Flask
* HTML / CSS

---

# 🎯 Learning Outcomes

Through this project, the following concepts are demonstrated:

* End-to-end Machine Learning workflow
* Data preprocessing and feature engineering
* Regularization techniques (Ridge, Lasso, ElasticNet)
* Model evaluation techniques
* Deployment of ML models using Flask
* Building simple ML web applications

---

# 📌 Future Improvements

Possible improvements for this project:

* Deploy the application using **Docker**
* Host the model on **AWS / Render / Railway**
* Add **interactive visualizations**
* Include **automatic input validation**
* Use **REST API for predictions**

---

# 👨‍💻 Author

Shibam Sadhukhan

Machine Learning Enthusiast | Data Science Learner

---

# ⭐ If you find this project useful

Please consider **starring the repository** on GitHub.
