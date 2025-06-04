#  Employee Management System with Weather Integration

A Python-based desktop GUI application built using **Tkinter** for managing employee records, integrated with **MongoDB** for data storage and **OpenWeatherMap API** to fetch current weather and location data.

---

##  Features

- **CRUD Operations**:
  - Add, View, Update, and Delete Employee records.
  - Data is stored in a local MongoDB database (`33oct` → `employe` collection).

- **Real-time Weather Info**:
  - Automatically displays current **temperature** and **city name** (hardcoded as Kalyan) using OpenWeatherMap API.

- **Top 5 Salaried Chart**:
  - Displays a bar chart of top 5 employees with the highest salaries using **matplotlib**.

- **Data Validation**:
  - Robust input validation for Employee ID, Name, and Salary.
  - Prevents entry of special characters, alphabets in salary, and numbers in name fields.

---

##  Technologies Used

- **Python 3**
- **Tkinter** – GUI framework
- **MongoDB (pymongo)** – NoSQL Database
- **OpenWeatherMap API** – for real-time weather
- **Matplotlib** – for chart plotting
- **Requests** – for API communication
- **Regular Expressions (re)** – for input validation

---

##  Requirements

Make sure to install the following Python packages:
```bash
pip install pymongo matplotlib requests
```

Also ensure **MongoDB** is running locally on port `27017`.

---

##  Screens

-  Add Employee
-  View All Employees
-  Update Employee
-  Delete Employee
-  Top 5 Salaried Chart
-  Weather + Location (displayed on the main dashboard)

---

##  API Key Setup

This app uses OpenWeatherMap's free API:
- Replace the `appid` value in the script with your personal API key from [openweathermap.org](https://openweathermap.org/).

```python
url = "https://api.openweathermap.org/data/2.5/weather?q=kalyan&appid=YOUR_API_KEY"
```

---

##  Running the Application

```bash
python p1.py
```

---

##  Notes

- The city name is **hardcoded** as `"kalyan"` for temperature and location display.
- Data validation is **strictly enforced** to ensure clean records in the database.

---

##  License

This project is free to use and modify for academic or personal use.
