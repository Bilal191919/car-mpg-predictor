🚗 Car MPG Predictor — Machine Learning Web App

A full-stack Machine Learning Web Application built with Flask and Random Forest Regression to predict a car’s Miles Per Gallon (MPG).
Users can upload their own CSV dataset, train a model, visualize feature importance, and generate real-time MPG predictions through an interactive UI.

⭐ Features
🔧 Machine Learning

Train model using any custom CSV dataset

Random Forest Regression for accurate MPG prediction

Automatic label encoding for categorical features

Displays R² Score and MAE after training

Feature importance graph (Chart.js)

🎛️ Frontend

Responsive and modern UI (HTML + CSS)

Dark/Light theme toggle

Dropdown inputs auto-load unique values from trained model

Real-time predictions with live result card

📝 Prediction History

Every prediction is stored in prediction_history.csv

View history in the UI

Download history as CSV

Auto-refresh table

📂 Supported Features for Prediction

Cylinders

Displacement

Year

Make

Fuel Type

Transmission

🛠️ Installation & Setup
1️⃣ Clone the repository
git clone https://github.com/your-username/car-mpg-predictor.git
cd car-mpg-predictor

2️⃣ Install dependencies
pip install -r requirements.txt

3️⃣ Run the Flask app
python app.py

4️⃣ Open in browser
http://127.0.0.1:5000/

📁 Dataset Requirements

Your CSV file must include at least:

cylinders
displacement
year
make
fuel_type
transmission
combination_mpg   (OR both city_mpg & highway_mpg)


If combination_mpg is missing, the app auto-calculates:

(city_mpg + highway_mpg) / 2

📊 Model Performance Example

R² Score: 0.89

MAE: 2.4

Displayed automatically after training.

📈 Feature Importance Example

The app displays a bar chart showing how each feature contributes to MPG prediction.

🧠 Tech Stack

Python (Flask) – Backend

Random Forest Regression (Sklearn)

Pandas, NumPy – Data processing

Chart.js – Feature graph

HTML, CSS, JavaScript – Frontend

📜 File Structure
├── app.py
├── mpg_model.pkl
├── prediction_history.csv
├── requirements.txt
└── README.md

🚀 Future Improvements

Add model comparison (Linear Regression, XGBoost etc.)

Upload multiple datasets

API endpoint documentation

Save multiple model versions

📬 Contributing

Pull requests are welcome! Feel free to improve UI/UX or model performance.

📝 License

This project is open-source and free to use.
