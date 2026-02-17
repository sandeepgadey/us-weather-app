# US Weather App

A simple, responsive web application that displays current weather information for major US cities using the free Open-Meteo API.

## Features

- **City Selection** - Choose from 20 major US cities via dropdown menu
- Real-time weather data with automatic refresh
- Clean, modern interface with weather emojis
- Responsive design that works on desktop and mobile
- Displays temperature, weather description, humidity, wind speed, pressure, and visibility
- Auto-refresh every 10 minutes for selected city
- Manual refresh button
- **No API key required** - uses free Open-Meteo service

## Available Cities

The app includes weather data for these major US cities:
- Seattle, WA
- New York City, NY  
- Los Angeles, CA
- Chicago, IL
- Houston, TX
- Phoenix, AZ
- Philadelphia, PA
- San Antonio, TX
- San Diego, CA
- Dallas, TX
- Austin, TX
- Jacksonville, FL
- Fort Worth, TX
- Columbus, OH
- Charlotte, NC
- San Francisco, CA
- Indianapolis, IN
- Denver, CO
- Washington, DC
- Boston, MA

## How to Use

1. **Select a city** from the dropdown menu at the top of the weather card
2. **Weather data automatically refreshes** when you change cities
3. **Manual refresh** using the "Refresh Weather" button
4. **Auto-refresh** every 10 minutes for the currently selected city

## Setup Instructions

1. **No API key needed!** This app uses the free Open-Meteo API which doesn't require registration or API keys.

2. **Run the app:**
   - Simply open `index.html` in your web browser
   - Or run a local server: `python -m http.server 8000` and visit `http://localhost:8000`
   - The app will automatically load weather data for the default city (Seattle)

## Files Structure

```
Weather App/
├── index.html      # Main HTML structure
├── styles.css      # Styling and responsive design
├── script.js       # Weather data fetching and display logic
└── README.md       # This file
```

## Browser Requirements

- Any modern web browser (Chrome, Firefox, Safari, Edge)
- Internet connection for API calls

## Troubleshooting

**"Unable to load weather data" error:**
- Check your internet connection
- Check browser console (F12) for detailed error messages
- Try refreshing the page

## Customization

You can easily add more cities by modifying the `CITIES` object in `script.js`:

```javascript
const CITIES = {
    your_city: { 
        name: "Your City, ST", 
        lat: 40.7128, 
        lon: -74.0060, 
        timezone: "America/New_York" 
    },
    // ... other cities
};
```

Then add the corresponding option to the HTML select element in `index.html`:

```html
<option value="your_city">Your City, ST</option>
```

## API Information

This app uses the Open-Meteo Weather API:
- Website: https://open-meteo.com/
- Completely free with no API key required
- No rate limits for non-commercial use
- High-quality weather data from national weather services

## License

This project is open source and available under the MIT License.