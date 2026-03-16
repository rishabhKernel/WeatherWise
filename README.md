# ⛅ WeatherWise

**WeatherWise** is a sleek, responsive, and user-friendly web application designed to provide real-time weather information. Built using HTML, CSS, and Vanilla JavaScript, it interacts with the OpenWeatherMap API to fetch and display accurate meteorological data based on either the user's current location or a specific city search.

## 🛠️ Tech Stack

*   **HTML5**
*   **CSS3**
*   **JavaScript (Vanilla)**

## 🌟 Key Features

### 1. 📍 Location-Based Weather (Your Weather Tab)
*   **Geolocation API Integration:** Asks for the user's permission to access their geographical coordinates (latitude and longitude).
*   **Automatic Fetching:** Once granted, it automatically fetches and displays the current weather for that exact location.
*   **Session Storage:** Saves the user's coordinates in `sessionStorage` so they don't have to re-grant permission every time they reload the page during the same session.

### 2. 🔍 Global City Search (Search Weather Tab)
*   **Search Functionality:** Allows users to input any city name globally.
*   **Dynamic Data Retrieval:** Fetches real-time weather data for the searched city using the OpenWeatherMap API's query parameter.

### 3. 📊 Comprehensive Weather Metrics
The application displays a detailed overview of the weather conditions:
*   **City Name & Country Flag:** Displays the searched/located city alongside its corresponding national flag (fetched via the FlagCDN API).
*   **Weather Description:** A brief textual description of the weather (e.g., "clear sky", "light rain").
*   **Weather Icon:** A visual representation of the current weather condition provided by OpenWeatherMap.
*   **Temperature:** Current temperature displayed in Celsius (°C).
*   **Wind Speed:** Current wind speed measured in meters per second (m/s).
*   **Humidity:** Air humidity percentage (%).
*   **Cloudiness:** Cloud cover percentage (%).

### 4. 💫 Intuitive UI & UX
*   **Tabbed Interface:** Smoothly transition between viewing "Your Weather" and searching for a specific city.
*   **Loading States:** Features a custom loading animation (GIF) that displays while API requests are pending, ensuring the user knows the app is working.
*   **Error Handling (Basic):** Includes structural scaffolding for handling API errors (e.g., city not found or network issues).

## 🛠️ Technologies & Tools Used

*   **HTML5:** Semantic markup defining the application's structure.
*   **CSS3:** Custom styling featuring Flexbox, Grid, custom properties (variables), media queries, and sophisticated background gradients.
*   **Vanilla JavaScript (ES6+):** 
    *   DOM Manipulation (selecting elements, adding/removing classes).
    *   Event Listeners (clicks, form submissions).
    *   Asynchronous Programming (`async/await`, `fetch` API for network requests).
    *   Geolocation API (`navigator.geolocation`).
    *   Session Storage API (`sessionStorage`).
*   **APIs:**
    *   [OpenWeatherMap API](https://openweathermap.org/api): To fetch real-time weather data.
    *   [FlagCDN](https://flagcdn.com/): To display country flags based on the country code returned by OpenWeatherMap.

## 📂 Project Structure

```text
WeatherWise-main/
│
├── index.html       # The main HTML structure
├── styles.css       # All styling rules and layout configurations
├── index.js         # Core application logic and API interactions
├── images/          # Directory containing all graphical assets
│   ├── cloud.png
│   ├── humidity.png
│   ├── loading.gif
│   ├── location.png
│   ├── search.png
│   └── wind.png
└── README.md        # Project documentation (this file)
```

## 🚀 How to Run the Project Locally

Running WeatherWise is incredibly straightforward as it doesn't require complex build steps or a dedicated backend server.

1.  **Clone or Download:**
    Clone the repository using Git or download the ZIP file and extract it.
    ```bash
    git clone <repository-url>
    ```

2.  **Open the Application:**
    Navigate to the project directory and open the `index.html` file directly in your preferred modern web browser (Chrome, Firefox, Edge, Safari).
    
    *Optional:* You can also use a simple static server like the "Live Server" extension in VS Code for a better development experience.

## 🔑 Important Note: OpenWeatherMap API Key

This application relies on the OpenWeatherMap API.

The `index.js` file currently contains an API key: 
`const API_KEY = "d1845658f92b31c64bd94f06f7188c9c";`

**⚠️ For developers cloning this project:** 
While this key might work temporarily for demonstration purposes, it is highly recommended that you generate your own **free API key** to avoid rate limiting or sudden service interruptions.

1.  Go to [OpenWeatherMap](https://openweathermap.org/) and create an account.
2.  Navigate to your profile and generate a new API key.
3.  Replace the string value of the `API_KEY` variable inside `index.js` with your newly generated key.

## 🧠 What I Learned Building This

This project served as an excellent practical exercise in modern web development concepts:
*   Deepened understanding of **Asynchronous JavaScript** by extensively using `async` and `await` with the `fetch` API.
*   Mastered DOM manipulation for creating dynamic, interactive user interfaces without relying on a framework like React.
*   Gained practical experience working with the browser's **Geolocation API** and handling user permissions.
*   Learned how to use **Session Storage** to persist small amounts of data across page reloads.
*   Improved CSS layout skills using modern techniques to create a clean, glass-morphism style interface.
