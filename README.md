# 🚗 Car Resale Value Prediction

## 📝 Project Overview

**Car Resale Value Prediction** is a small-scale machine learning project that predicts the resale value of a car based on several features such as:

* Original price
* Kilometers driven
* Seller type
* Transmission type
* Years of usage

The project integrates a **Python-based machine learning model** with a **Node.js + Express** web interface for user interaction.

---

## 💻 Technologies Used

* **Python 3** — Core language for model training
* **Scikit-learn (sklearn)** — Used to train the prediction model using `RandomForestRegressor`
* **Pandas & NumPy** — Data preprocessing and numerical analysis
* **Node.js & Express.js** — Backend framework for web integration
* **EJS** — Frontend templating engine

---

## ⚙️ Prerequisites

Before running the project, make sure you have the following installed:

* `Python 3` (or `python` on Windows)
* `Node.js` and `npm`
* Required Python libraries:

  ```bash
  pip install sklearn pandas numpy
  ```

---

## 🚀 How to Run the Project

### Step 1: Download the Repository

Clone or download this repository to your local system:

```bash
git clone https://github.com/Bhabashis001/Car-Resale-Value-Prediction-using-Node.JS
```

### Step 2: Navigate to the Project Directory

```bash
cd Car-Resale-Value-Prediction/
```

### Step 3: Train the Prediction Model

```bash
python3 price_prediction.py   # Use 'python price_prediction.py' on Windows
```

### Step 4: Start the Web Application

```bash
cd Website/
npm start
```

### Step 5: Access the Application

Open your browser and go to:

```
http://localhost:3000
```

### Step 6: Predict Resale Value

Fill in the required details such as:

* Purchase price
* KMs driven
* Year of purchase
* Fuel type
* Transmission type
* Seller type

Then click **Predict** to view your car’s estimated resale value.

---

## 🧩 Troubleshooting

### 1️⃣ Error: `child_process` on `script.py`

If you’re running this on **Windows**, modify the command in `app.js`:

```js
// Change this line:
const pythonProcess = spawn('python3', ['script.py']);

// To this:
const pythonProcess = spawn('python', ['script.py']);
```

### 2️⃣ App Keeps Loading (Waiting for localhost)

If the app does not respond:

1. Delete the file `model.sav` in the main folder.
2. Rerun:

   ```bash
   python price_prediction.py
   ```

   This will retrain and refresh the model (takes about 10–30 seconds).

---

## 🧠 About the Model

The model is based on **Random Forest Regression**, a robust ensemble learning method that handles nonlinear relationships effectively.
The dataset was obtained from **Kaggle**, preprocessed using **Pandas**, and trained using **Scikit-learn**.

