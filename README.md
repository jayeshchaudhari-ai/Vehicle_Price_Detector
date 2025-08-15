# Vehicle_Price_Predictor
The Vehicle Price Predictor uses machine learning to estimate a car’s market value based on details like make, model, year, engine, mileage, and more. With a simple web form and instant results, it helps buyers, sellers, and dealers make informed pricing decisions quickly and accurately. Ask ChatGPT

🚗 Vehicle Price Predictor








A web application powered by Machine Learning that estimates the market value of a vehicle based on its specifications.
Designed using Python, Flask, scikit-learn, HTML, and CSS.

📋 Contents

💡 Highlights

📊 Data Source

🛠 Technologies

📂 Directory Layout

⚙ How to Install

▶ How to Use

📌 Sample Results

🎯 How to Customize

🖼 Interface Preview

📜 License

💡 Highlights

✅ Accepts multiple inputs: make, model, year, engine, fuel type, mileage, trim, body style, colors, drivetrain, etc.
✅ User-friendly, interactive form.
✅ Instant price prediction without refreshing the page.
✅ Built-in feature engineering and preprocessing.
✅ Fully supports custom datasets.
✅ Includes a pre-trained RandomForestRegressor model.

📊 Data Source

The training dataset consists of:

Brand & Model – manufacturer and variant.

Manufacturing Year – vehicle’s production year.

Engine Details – displacement, turbo, or electric type.

Mileage – distance traveled.

Fuel & Transmission – type of fuel and gearbox.

Trim & Body – specific version and body category.

Colors – exterior and interior shades.

Drivetrain – such as FWD, AWD, or 4WD.

Price – target value (actual selling price).

🛠 Technologies
Layer	Stack Used
Backend	Python, Flask
ML Model	scikit-learn, pandas, numpy
Frontend	HTML5, CSS3
Storage	joblib .pkl
Algorithm	RandomForestRegressor
📂 Directory Layout
vehicle_price_predictor/
│── app.py                # Flask application
│── train_model.py         # ML training script
│── vehicle_price_model.pkl # Pre-trained model
│── templates/
│    └── index.html        # Web form
│── static/
│    └── car.svg           # Logo / icon
│── dataset.csv            # Dataset
│── requirements.txt       # Dependencies
│── README.md              # Documentation

⚙ How to Install

1️⃣ Clone the repository:

git clone https://github.com/jayeshchaudhari-ai/Vehicle_Price_Predictor.git
cd Vehicle_Price_Predictor


2️⃣ Install dependencies:

pip install -r requirements.txt


3️⃣ (Optional) Retrain the model:

python train_model.py


4️⃣ Start the Flask server:

python app.py


5️⃣ Open in your browser:

http://127.0.0.1:5000/

▶ How to Use

Open the web form.

Enter the vehicle details.

Click Predict Price.

View the estimated market value instantly.

📌 Sample Results
Make	Model	Year	Engine	Mileage	Fuel	Predicted Price
Toyota	Camry	2018	2.5L	40000	Gasoline	$16,500
Tesla	Model 3	2022	Electric	5000	Electric	$44,200
Ford	F-150	2020	3.5L	25000	Gasoline	$38,900
🎯 How to Customize

Replace dataset.csv with your own data.

Modify train_model.py to try different ML algorithms.

Adjust currency formatting in app.py.

🙌 Developed by Jayesh Chaudhari using Python, Flask, and scikit-learn.
