# 🌦️ Console Weather App

A console-based application that fetches **real-time weather data** from multiple providers using automatic **IP-based location detection** or **manual city input**. It integrates with **OpenWeatherMap**, **WeatherStack**, and **IpStack** APIs to provide accurate weather information with intelligent **caching**, **rate limiting**, and **error handling**.

---

## 📌 Features

-  **Location Detection**  
  - Automatic location via **IP address** (no manual IP input needed)  
  - Manual city name input  
  - Displays latitude, longitude, and city name

-  **Weather Data Integration**  
  - Weather fetched from **OpenWeatherMap** and **WeatherStack**  
  - Displays temperature (in Celsius), weather conditions, and location  
  - Shows which API was used for the data

-  **Caching System**  
  - Weather data cached for **10 minutes** to reduce API calls  
  - Returns cached results if available

-  **Rate Limiting**  
  - Enforces a **30-second cooldown** per provider  
  - Automatically switches to the backup provider when limit is hit  
  - Provides real-time user feedback

-  **Robust Error Handling**  
  - Gracefully handles network failures, API timeouts, and invalid inputs  
  - Clear messages for debugging and user clarity

-  **Console Interface**  
  - Interactive command-line UI  
  - Clear menu for location method selection  
  - Clean and readable output of weather data

---

##  Tech Stack

- **Language**: Java 
- **APIs Used**:
  - [OpenWeatherMap](https://openweathermap.org/api)
  - [WeatherStack](https://weatherstack.com/)
  - [IpStack](https://ipstack.com/)
  - [ipify](https://www.ipify.org/) for external IP detection  
- **Async Requests**: Asynchronous API handling for non-blocking operations  
- **HTTP Client**: Used for communicating with APIs (e.g., `HttpClient`, `OkHttp`, `requests`, etc.)

---


