# Weather App (Next.js - Internship Project)

This is a simple weather application built with Next.js, developed as an internship project. It allows users to search for weather information by city name, utilizing the OpenWeatherMap API for real-time data.

**Important Note:** This project is intended for educational purposes as part of an internship. It does not include an `.env` file for API key management or a formal license.

## Features

-   **Search Functionality:** Users can enter a city name in the search bar and retrieve weather information.
-   **Real-time Weather Data:** Displays current weather conditions, temperature, humidity, wind speed, and weather icon.
-   **Responsive UI:** Designed to be clean, modern, and responsive across different devices, using Next.js's built-in CSS modules or styled-components.
-   **Loading State:** Shows a loading indicator while fetching data from the API.
-   **Error Handling:** Displays appropriate error messages for invalid city names or API failures.
-   **Metric Units:** Displays temperature in Celsius (°C) and wind speed in kilometers per hour (km/h).
-   **Next.js Features:** Leverages Next.js features like server-side rendering (SSR) or static site generation (SSG) for performance optimization (if applicable).

## Technologies Used

-   Next.js
-   React
-   OpenWeatherMap API
-   `fetch` or `axios` (for HTTP requests)
-   CSS Modules or Styled Components (for styling)

## Getting Started

1.  **Clone the Repository:**

    ```bash
    git clone <repository_url>
    ```

2.  **Install Dependencies:**

    ```bash
    cd <repository_directory>
    npm install
    # or
    yarn install
    # or
    pnpm install
    ```

3.  **Configure API Key (Directly in Code - NOT Recommended for Production):**

    -   **For this internship project, you will place your API key directly into the javascript file, this is not a secure practice, and should not be used in real world applications.**
    -   Open the appropriate component file (e.g., `pages/index.js` or where you make the API call).
    -   Replace `{YOUR_API_KEY}` in the API URL with your actual API key.

    ```javascript
    const apiKey = 'YOUR_API_KEY'; // Replace with your API key - Internship only!
    const apiUrl = `https://api.openweathermap.org/data/2.5/weather?q=${city}&appid=${apiKey}&units=metric`;
    ```
    -   **Important:** In a real application, use environment variables or a secure configuration method.

4.  **Run the Development Server:**

    ```bash
    npm run dev
    # or
    yarn dev
    # or
    pnpm dev
    ```

5.  **Open in Browser:**

    -   Open your browser and navigate to `http://localhost:3000`.

## Usage

1.  Enter the name of a city in the search bar.
2.  Click the "Submit" button or press Enter.
3.  The weather information for the specified city will be displayed.
4.  If an error occurs (e.g., invalid city name or API failure), an error message will be shown.

## API Integration

-   The application uses the OpenWeatherMap Current Weather API to fetch weather data.
-   API URL: `https://api.openweathermap.org/data/2.5/weather?q={city}&appid={YOUR_API_KEY}&units=metric`
-   The `units=metric` parameter ensures that the temperature is displayed in Celsius and wind speed in kilometers per hour.
-   `fetch` or `axios` is used to make HTTP requests to the API.
-   Error handling is implemented to manage API failures and invalid city names.

## UI Design

-   The user interface is designed to be clean and modern, leveraging Next.js's styling capabilities.
-   It includes a search bar, submit button, and a weather info card.
-   The weather info card displays the following information:
    -   City Name
    -   Current Temperature (°C)
    -   Weather Condition (e.g., Sunny, Rainy, Snow)
    -   Humidity (%)
    -   Wind Speed (km/h)
    -   Weather Icon (provided by the API)
-   A loading state is displayed while fetching data.
-   Error messages are displayed for invalid input or API errors.

## Next.js Specifics

-   **Routing:** Utilizes Next.js's file-based routing.
-   **Styling:** Uses CSS Modules or styled-components for component-scoped styling.
-   **Data Fetching:** Implements data fetching using `fetch` or `axios` within Next.js components.
-   **Performance Optimization:** Potential use of SSR or SSG depending on the implementation.

## Future Improvements (Beyond Internship Scope)

-   Add support for displaying weather forecasts.
-   Implement location-based weather retrieval.
-   Enhance the UI with more detailed weather information.
-   Add support for different unit systems (e.g., Fahrenheit).
-   Improve Accessibility.
-   Implement better state management.
-   **Securely store API keys using environment variables or a secrets management solution.**
-   **Add a License.**

## Contributing

As this is an internship project, contributions are not expected.