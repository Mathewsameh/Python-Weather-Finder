# 🌦️ Weather Finder

A simple Python application that retrieves the current temperature of a city using the **Open-Meteo API**.

The program allows users to enter a city name, find its geographical coordinates, and retrieve the current temperature in Celsius.

## 📌 Project Overview

Weather Finder is a beginner-friendly Python project designed to practice working with external APIs, handling JSON responses, and processing user input.

It uses the Open-Meteo Geocoding API to find a city's location and the Open-Meteo Forecast API to retrieve its current weather data.

## ✨ Features

- 🌍 Search for a city by name.
- 🏳️ Display the city's name and country.
- 📍 Retrieve geographical coordinates (latitude and longitude).
- 🌡️ Display the current temperature in Celsius.
- ⚠️ Handle cases where a city cannot be found.
- 🛡️ Handle HTTP request errors when retrieving weather data.

## 🛠️ Technologies Used

- **Python 3**
- **Requests Library**
- **Open-Meteo Geocoding API**
- **Open-Meteo Forecast API**
- **JSON**
- **Exception Handling**

## 📋 Requirements

- Python 3.x
- An active internet connection.
- The `requests` library.

## 🚀 Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/weather-finder.git
```

Replace `YOUR-USERNAME` with your GitHub username.

### 2. Navigate to the Project Folder

```bash
cd weather-finder
```

### 3. Install Dependencies

```bash
pip install requests
```

### 4. Run the Program

```bash
python main.py
```

Make sure your Python file is named `main.py`, or replace it with your actual filename.

## 💻 Example Usage

```text
Enter your city: Cairo

City: Cairo
Country: Egypt
Temperature: 27.5 °C
```

*Note: The temperature above is an illustrative example, not a live weather reading. Actual results depend on the selected city and current weather conditions.*

## 🔄 How It Works

1. The program asks the user to enter a city name.
2. It sends a GET request to the Open-Meteo Geocoding API.
3. It checks whether the API returned any matching cities.
4. If no results are found, it displays a city-not-found error.
5. If a match is found, it extracts the city's name, country, latitude, and longitude.
6. It sends another GET request to the Open-Meteo Forecast API using the geographical coordinates.
7. It requests the current temperature using the `current=temperature_2m` parameter.
8. It checks the HTTP response for errors and displays the temperature in Celsius.

## 📚 What I Learned

Through this project, I practiced:

- Sending HTTP GET requests using Python.
- Passing query parameters to APIs.
- Working with two APIs in one application.
- Processing JSON responses and Python dictionaries.
- Understanding latitude and longitude.
- Checking whether API responses contain expected data.
- Handling exceptions with `try` and `except`.
- Using `raise_for_status()` to detect unsuccessful HTTP responses.

## 🔮 Future Improvements

- Display additional weather information, such as humidity and wind speed.
- Show the current weather conditions with descriptive labels.
- Allow users to choose between Celsius and Fahrenheit.
- Add request timeouts and more robust error handling to every API request.
- Handle multiple cities with the same name.
- Display a short weather forecast for the next few days.
- Build a graphical user interface.

## 📖 Useful Resources

- [Open-Meteo Official Website](https://open-meteo.com/)
- [Open-Meteo Geocoding API Documentation](https://open-meteo.com/en/docs/geocoding-api)
- [Open-Meteo Weather Forecast API Documentation](https://open-meteo.com/en/docs)
- [Python Requests Documentation](https://requests.readthedocs.io/en/latest/)

## 👨‍💻 Author

**YOUR NAME**

- GitHub: [@YOUR-USERNAME](https://github.com/YOUR-USERNAME)

---

⭐ If you find this project useful, consider giving the repository a star!
