# Stock-price-pipeline
A cloud-based real-time stock price data pipeline with a web analytics dashboard.

📌 Project Overview

This project is a cloud-based stock price data pipeline that fetches real-time stock data using Yahoo Finance, processes it, and visualizes key financial metrics on a web-based dashboard. The goal is to gain hands-on experience with cloud technologies, Python, and data processing while building an impressive portfolio project.

🚀 Tech Stack

Cloud Provider: AWS (S3, Lambda, DynamoDB, EC2)

Programming Language: Python

Data API: Yahoo Finance (yfinance library)

Web Framework: Flask (for the dashboard)

Data Processing: Pandas, NumPy

Visualization: Plotly, Chart.js

Automation: AWS CloudWatch Scheduler

Version Control: Git & GitHub

🎯 Features

Fetches real-time stock prices from Yahoo Finance.

Stores raw stock data in AWS S3.

Processes data (moving averages, daily returns) using AWS Lambda.

Stores processed data in AWS DynamoDB.

Displays interactive stock charts using Flask and Plotly.

Automates data fetching and processing with AWS CloudWatch Scheduler.

📊 Architecture Diagram

[Yahoo Finance API] → [AWS Lambda: Fetch Data] → [AWS S3: Store Raw Data] →
[AWS Lambda: Process Data] → [AWS DynamoDB: Store Processed Data] →
[Flask Dashboard on AWS EC2] → [User Views Stock Data]

🛠️ Setup Instructions

1️⃣ Prerequisites

AWS Account (Sign up)

Python 3.x installed

Git installed

Virtual environment setup (optional but recommended)

2️⃣ Clone the Repository

git clone https://github.com/yourusername/stock-price-pipeline.git
cd stock-price-pipeline

3️⃣ Install Dependencies

pip install -r requirements.txt

4️⃣ Set Up AWS Services

AWS S3: Create a bucket for storing raw stock data.

AWS Lambda: Create two functions for fetching and processing stock data.

AWS DynamoDB: Create a table with primary key StockSymbol and sort key Date.

AWS EC2: Launch an instance to host the Flask dashboard.

AWS CloudWatch Scheduler: Schedule Lambda to run at set intervals.

5️⃣ Run Locally (For Testing)

python app.py  # Runs the Flask dashboard locally

📌 Future Enhancements

Add user authentication for the dashboard.

Implement stock price alerts (email/SMS notifications).

Use machine learning to predict future stock prices.

Containerize the application using Docker.

Deploy using AWS Elastic Beanstalk for better scalability.

📜 License

This project is licensed under the MIT License. See the LICENSE file for details.
