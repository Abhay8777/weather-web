# 🌦️ Weather Web

A modern and responsive **Weather Web Application** built using **HTML, CSS, and JavaScript**.

The application allows users to search for a city and view its current weather information along with additional weather details and forecast information.

---

## 🔗 Repository

**GitHub:**  
https://github.com/Abhay8777/weather-web

---

## 📸 Project Preview

### 🔍 Search Screen

![Search City](screenshots/search.png)

### 🌤️ Weather Information

![Weather Information](screenshots/weather.png)

---

## ✨ Features

- 🔍 Search weather by city name
- 📍 Display city and location
- 🌡️ Display current temperature
- ☁️ Display current weather condition
- 💧 Display humidity
- 💨 Display wind speed
- 📅 Display upcoming weather forecast
- 🌦️ Dynamic weather icons
- ❌ Invalid city / error handling
- 📱 Responsive user interface
- 🎨 Modern glassmorphism UI
- ⚡ Dynamic data using JavaScript

---

# 🏗️ Project Architecture

The application follows a simple **Client-Side Web Architecture**.

```text
                         ┌──────────────────────┐
                         │        USER          │
                         │                      │
                         │   Enter City Name    │
                         └──────────┬───────────┘
                                    │
                                    ▼
                         ┌──────────────────────┐
                         │     index.html      │
                         │                      │
                         │   User Interface     │
                         └──────────┬───────────┘
                                    │
                                    ▼
                         ┌──────────────────────┐
                         │      script.js       │
                         │                      │
                         │  Application Logic   │
                         └──────────┬───────────┘
                                    │
                                    │ API Request
                                    ▼
                         ┌──────────────────────┐
                         │     Weather API      │
                         │                      │
                         │    Weather Data      │
                         └──────────┬───────────┘
                                    │
                                    │ JSON Response
                                    ▼
                         ┌──────────────────────┐
                         │      script.js       │
                         │                      │
                         │  Process API Data    │
                         └──────────┬───────────┘
                                    │
                                    ▼
                         ┌──────────────────────┐
                         │   DOM Manipulation   │
                         │                      │
                         │ Update Weather Data  │
                         └──────────┬───────────┘
                                    │
                                    ▼
                         ┌──────────────────────┐
                         │      style.css       │
                         │                      │
                         │  Display & Styling   │
                         └──────────┬───────────┘
                                    │
                                    ▼
                         ┌──────────────────────┐
                         │        USER          │
                         │                      │
                         │ Weather Information  │
                         └──────────────────────┘
```

---

# 📂 Folder Structure

```text
weather/
│
├── message/
│   │
│   ├── atmosphere.svg
│   ├── bg.jpg
│   ├── clear.svg
│   ├── clouds.svg
│   ├── drizzle.svg
│   ├── rain.svg
│   ├── snow.svg
│   ├── thunderstorm.svg
│   ├── search-city.png
│   └── not-found.png
│
├── screenshots/
│   ├── search.png
│   └── weather.png
│
├── index.html
├── style.css
├── script.js
└── README.md
```

---

# 🖥️ User Interface Architecture

The application interface is divided into several sections.

```text
┌─────────────────────────────────────┐
│        🌦️ WEATHER APPLICATION        │
├─────────────────────────────────────┤
│                                     │
│         🔍 Search City              │
│                                     │
├─────────────────────────────────────┤
│                                     │
│   📍 City                📅 Date    │
│                                     │
│          🌤️     28°C               │
│                 Clouds              │
│                                     │
├─────────────────────────────────────┤
│                                     │
│    💧 Humidity       💨 Wind Speed  │
│       83%               0 m/s       │
│                                     │
├─────────────────────────────────────┤
│                                     │
│          📅 Weather Forecast        │
│                                     │
│   ┌─────┐  ┌─────┐  ┌─────┐       │
│   │ Sep │  │ Sep │  │ Sep │       │
│   │ 19  │  │ 20  │  │ 21  │       │
│   │ 🌧️  │  │ 🌤️  │  │ ☀️  │       │
│   └─────┘  └─────┘  └─────┘       │
│                                     │
└─────────────────────────────────────┘
```

---

# 🔄 Application Workflow

The application works through the following process:

```text
User
 │
 │ Enter City
 ▼
Search Input
 │
 ▼
JavaScript Event Handler
 │
 ▼
Weather API Request
 │
 ▼
Weather API
 │
 │ JSON Response
 ▼
JavaScript Data Processing
 │
 ▼
DOM Manipulation
 │
 ▼
Weather Information
 │
 ▼
User
```

---

# 🌐 Data Flow

```text
                    ┌───────────────┐
                    │     USER      │
                    └───────┬───────┘
                            │
                            │ City Name
                            ▼
                    ┌───────────────┐
                    │  User Input   │
                    └───────┬───────┘
                            │
                            ▼
                    ┌───────────────┐
                    │  script.js    │
                    └───────┬───────┘
                            │
                            │ API Request
                            ▼
                    ┌───────────────┐
                    │  Weather API  │
                    └───────┬───────┘
                            │
                            │ JSON Response
                            ▼
                    ┌───────────────┐
                    │  Data         │
                    │  Processing   │
                    └───────┬───────┘
                            │
                            ▼
                    ┌───────────────┐
                    │ DOM Update    │
                    └───────┬───────┘
                            │
                            ▼
                    ┌───────────────┐
                    │ Weather UI    │
                    └───────────────┘
```

---

# 🧩 Architecture Components

## 1. HTML Layer — `index.html`

Responsible for the structure of the application.

It contains:

- Search input
- Search button
- Location information
- Current date
- Temperature
- Weather condition
- Humidity
- Wind speed
- Forecast section
- Weather icons

---

## 2. CSS Layer — `style.css`

Responsible for the visual presentation of the application.

It handles:

- Layout
- Colors
- Typography
- Glassmorphism effect
- Search bar styling
- Weather card
- Forecast cards
- Responsive design
- Background
- Spacing and alignment

---

## 3. JavaScript Layer — `script.js`

Responsible for the functionality and application logic.

It handles:

- User input
- Search events
- API requests
- JSON responses
- Weather data processing
- DOM manipulation
- Dynamic weather icons
- Forecast information
- Error handling

---

## 4. Assets Layer — `message/`

Contains the visual assets used by the application.

```text
message/
│
├── atmosphere.svg
├── clear.svg
├── clouds.svg
├── drizzle.svg
├── rain.svg
├── snow.svg
├── thunderstorm.svg
├── bg.jpg
├── search-city.png
└── not-found.png
```

---

# 🌦️ Weather Data Display

After searching for a city, the application displays weather information such as:

```text
📍 Location
📅 Current Date
🌡️ Temperature
☁️ Weather Condition
💧 Humidity
💨 Wind Speed
📅 Weather Forecast
```

---

# 🎨 Weather Assets

Different weather conditions use different icons.

| Condition | Asset |
|-----------|-------|
| Clear | `clear.svg` |
| Clouds | `clouds.svg` |
| Rain | `rain.svg` |
| Drizzle | `drizzle.svg` |
| Snow | `snow.svg` |
| Thunderstorm | `thunderstorm.svg` |
| Atmosphere | `atmosphere.svg` |

---

# 🛠️ Technologies Used

| Technology | Purpose |
|------------|---------|
| HTML5 | Application structure |
| CSS3 | Styling and responsive design |
| JavaScript | Application logic |
| Weather API | Fetching weather data |
| SVG | Weather icons |
| Git | Version control |
| GitHub | Repository hosting |
| VS Code | Development environment |

---

# 📱 Responsive Design

The application is designed to work across different screen sizes.

```text
Desktop
   ↓
Laptop
   ↓
Tablet
   ↓
Mobile
```

The layout adjusts according to the screen size to provide a consistent user experience.

---

# ⚠️ Error Handling

The application handles common situations such as:

```text
Empty Input
     ↓
Invalid City
     ↓
City Not Found
     ↓
API Error
     ↓
Network Error
```

The application displays an appropriate error state instead of leaving the interface blank.

---

# 🔐 API Security

If the application uses an API key, the key should not be publicly exposed in the source code.

For example:

```javascript
const API_KEY = "YOUR_API_KEY";
```

For production applications, API credentials should be stored securely using environment variables or a backend service.

---

# 🚀 How to Run

### 1. Clone the repository

```bash
git clone https://github.com/Abhay8777/weather-web.git
```

### 2. Open the project

```bash
cd weather-web
```

### 3. Open in VS Code

```bash
code .
```

### 4. Run the application

Open `index.html` using **Live Server** in VS Code.

---

# 📈 Future Improvements

- 📍 Current location weather
- 📅 Extended weather forecast
- 🌡️ Celsius / Fahrenheit conversion
- 🌙 Dark / Light mode
- ⭐ Favorite cities
- 🕒 Search history
- 🌍 Multiple location support
- 📊 Weather charts
- 🌅 Sunrise and sunset information
- 📱 Progressive Web App support

---

# 🎯 Learning Objectives

This project demonstrates practical implementation of:

- HTML5
- CSS3
- JavaScript
- DOM Manipulation
- Event Handling
- API Integration
- Fetch API
- JSON Data Handling
- Asynchronous JavaScript
- Error Handling
- Responsive Web Design
- Git & GitHub

---

# 💡 Key Concepts Used

```text
HTML
 │
 ├── Page Structure
 │
 ▼
CSS
 │
 ├── UI Design
 ├── Responsive Layout
 └── Glassmorphism
 │
 ▼
JavaScript
 │
 ├── Events
 ├── DOM Manipulation
 ├── Fetch API
 ├── JSON
 └── Error Handling
 │
 ▼
Weather API
 │
 └── Real-Time Weather Data
```

---

# 👨‍💻 Author

## Abhay Mishra

**B.Tech — Computer Science Engineering**

GitHub:  
https://github.com/Abhay8777

---

# 📄 License

This project is created for educational and learning purposes.

---

⭐ **If you found this project useful, consider giving the repository a star!**
