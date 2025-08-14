# Local-Food-Wastage-Management-System
Project Description

The Local Food Wastage Management System is a Python-based web application that helps reduce food wastage by connecting food providers (restaurants, hotels, households) with receivers (NGOs, needy individuals).
The system enables users to list surplus food, manage availability, and track claims in real-time.
It also provides data analytics and visualizations to monitor donations and claim trends.

This project was developed using Streamlit for the web interface, SQLite for the database, and ngrok to make the application accessible online from Google Colab.

🚀 Features

Add, View, Update, Delete (CRUD) food listings

Filter listings by city and food type

SQL queries for quick analytics

Charts & Visualizations using Matplotlib

Run online via Google Colab + ngrok

Lightweight (no heavy installations)

🛠️ Tools & Technologies Used

Tool / Library	Purpose
Python	Core programming language
Streamlit	Web application framework
SQLite	Lightweight database for storing data
Pandas	Data manipulation and filtering
Matplotlib	Data visualization
ngrok	Makes local app accessible online
Google Colab	Runs app in the cloud without setup

Database Tables
1. Providers
Field	Type
Provider_ID	INTEGER (PK)
Name	TEXT
City	TEXT
Contact	TEXT
Provider_Type	TEXT
Email	TEXT
2. Food Listings
Field	Type
Food_ID	INTEGER (PK)
Food_Name	TEXT
Quantity	INTEGER
Expiry_Date	TEXT
Provider_ID	INTEGER (FK)
Location	TEXT
Food_Type	TEXT
Meal_Type	TEXT
3. Receivers
Field	Type
Receiver_ID	INTEGER (PK)
Name	TEXT
City	TEXT
Contact	TEXT
4. Claims
Field	Type
Claim_ID	INTEGER (PK)
Food_ID	INTEGER (FK)
Receiver_ID	INTEGER (FK)
Status	TEXT
