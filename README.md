Weather API Flask Application

🌍 Overview

This project is a simple Flask-based Weather API, which provides temperature data for various weather stations. The data is loaded from CSV files and made accessible through API endpoints.

📌 Features

Retrieve temperature data for a specific station and date.

Get all available data for a weather station.

Fetch yearly temperature records for a station.

Render an HTML page displaying available weather stations.

🛠 Technologies Used

Python (Flask, Pandas)

HTML/CSS (for basic front-end pages)

CSV data files (used for weather data storage)

🚀 Installation & Setup

1️⃣ Clone the Repository:

git clone [https://github.com/your-username/weather-api.git](https://github.com/PolytechnicCoder/weather-api)
cd weather-api

2️⃣ Create a Virtual Environment:

python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate

3️⃣ Install Dependencies:

pip install -r requirements.txt

4️⃣ Run the Application:

python main.py

By default, the application will run on http://127.0.0.1:5000/.

🌐 API Endpoints

🔹 Get Temperature for a Specific Date & Station

GET /api/v1/<station>/<date>

Response:

{
  "station": "1",
  "date": "2023-03-15",
  "temperature": 10.5
}

🔹 Get All Data for a Station

GET /api/v1/<station>

Returns all temperature records for the given station.

🔹 Get Yearly Data for a Station

GET /api/v1/yearly/<station>/<year>

Returns all temperature records for a specific year.

📂 Project Structure

app-6-your-wether-api/
│── static/            # CSS, JavaScript files
│── templates/         # HTML templates
│── data_small/        # CSV files containing weather data
│── main.py            # Flask application
│── about.html         # Additional page
│── tutorial.html      # Guide page
│── .gitignore         # Git ignored files
│── requirements.txt   # Python dependencies

🌦 Weather API - Developed with Flask & Python
