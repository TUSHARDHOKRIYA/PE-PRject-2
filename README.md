# 🌤️ WeatherVista - Prompt Engineering Weather App

WeatherVista is a modern, responsive weather forecast application designed using **prompt engineering** principles. It fetches real-time weather data using the [WeatherAPI.com](https://www.weatherapi.com/) and displays it interactively based on user queries.

## 🚀 Features

- **🌈 Dynamic Weather Display**  
  Icons and background colors change according to weather conditions.

- **📱 Responsive UI**  
  Optimized for both desktop and mobile devices.

- **🎞️ Interactive Animations**  
  Animated icons and smooth background transitions enhance user experience.

- **⚠️ Robust Error Handling**  
  Provides clear, user-friendly messages for invalid inputs and fetch errors.

- **📊 Detailed Weather Data**  
  Displays temperature, humidity, wind speed, pressure, precipitation, and UV index.

---

## 🧠 Prompt Engineering Components

### 1. User Input Prompts
Validates city name input before fetching data.

```javascript
if (!cityInput) {
    return "Please enter a city name (e.g., 'London,GB')";
}
if (!/^[a-zA-Z\s,]+$/.test(cityInput)) {
    return "Please enter a valid city name (letters, spaces, or commas only)";
}



Maps weather conditions to specific UI styles:

javascript
Copy
Edit
const weatherStyles = {
  'Sunny': { icon: 'fas fa-sun', bg: 'bg-gradient-to-br from-amber-100 to-amber-300', color: 'text-amber-600' },
  'Clear': { icon: 'fas fa-sun', bg: 'bg-gradient-to-br from-blue-100 to-blue-300', color: 'text-blue-600' },
  'default': { icon: 'fas fa-globe-americas', bg: 'bg-gradient-to-br from-blue-100 to-blue-300', color: 'text-blue-600' }
};

