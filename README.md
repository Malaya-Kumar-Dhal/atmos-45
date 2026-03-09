# 🌤️ Atmos — Real-Time Weather App

A beautiful, fully client-side weather application built in a single HTML file. No server, no API keys, no sign-up required. Just open it in any browser and search any city on Earth.

---

## ✨ Features

### 🔍 Smart City Search
- Type any city name and press **Enter** to search
- Results are fetched simultaneously from **3 geocoding APIs** (Nominatim, Photon, Open-Meteo) and merged — ensuring near-complete global coverage including small towns, villages, and non-English place names
- Matching locations are displayed as a clear pick-list so you always choose the exact place you mean

### ⭐ Favorites & History
- **Save cities** with the star button — favorites persist across sessions via localStorage
- **Recent searches** are automatically tracked and shown as quick-tap chips for fast re-access

### 🌡️ Current Conditions
- Live temperature with **feels-like**, daily high/low
- Weather condition with animated emoji icon
- **°C / °F toggle** that instantly updates all values across the entire page

### ⚠️ Weather Alerts
- Automatic warning banners for dangerous conditions: thunderstorms, violent rain, extreme heat, extreme cold, and very strong winds

### 📊 Stats Panel
- Relative humidity
- Wind speed (km/h or mph)
- Visibility (km or mi)
- Atmospheric pressure (hPa)

### 📈 24-Hour Temperature Chart
- SVG sparkline showing the temperature curve across the next 24 hours with labeled time markers

### ⏰ Hourly Forecast
- Scrollable hour-by-hour breakdown for the next 24 hours with weather icons and rain probability

### 📅 7-Day Forecast
- Daily high/low temperatures, weather condition and icon for the next 7 days

### 🌬️ Air Quality Index (AQI)
- Live European AQI score from the Open-Meteo Air Quality API
- Color-coded rating: Good → Fair → Moderate → Poor → Very Poor → Extremely Poor
- Breakdown of individual pollutants: **PM2.5**, **PM10**, **NO₂**

### 🧭 Wind Compass
- Animated compass rose that rotates to show real wind direction in degrees
- Cardinal direction label (N, NE, E, etc.) and wind speed

### ☀️ UV Index
- Current UV index with a gradient bar indicator and plain-English risk label (Low / Moderate / High / Very High / Extreme)

### 🌙 Moon Phase
- Calculated moon phase for today with emoji icon, phase name, and days until the next full moon

### 🌅 Sunrise & Sunset
- Today's sunrise and sunset times with an animated arc showing the sun's current position in the sky
- Total daylight duration for the day

### 👕 What to Wear & Do
- Smart clothing and activity suggestions generated from the current temperature, weather code, wind speed, and humidity — e.g. umbrella reminders, sunscreen, cycling or running conditions, heavy coat advice

### 🌧️ 7-Day Precipitation
- Bar chart showing daily rainfall/snowfall in mm with actual values labelled per bar

### 🎨 Animated Background
- Live canvas particle system that adapts to weather: **stars** for clear skies, **rain streaks** for rain, **snowflakes** for snow

---

## 🛰️ APIs Used

All APIs are **free and require no API key**.

| API | Purpose |
|-----|---------|
| [Open-Meteo Forecast](https://open-meteo.com/) | Current weather, hourly & daily forecasts |
| [Open-Meteo Air Quality](https://open-meteo.com/en/docs/air-quality-api) | AQI, PM2.5, PM10, NO₂ |
| [Open-Meteo Geocoding](https://open-meteo.com/en/docs/geocoding-api) | City search (source 1 of 3) |
| [Nominatim / OpenStreetMap](https://nominatim.org/) | City search (source 2 of 3) |
| [Photon by Komoot](https://photon.komoot.io/) | City search (source 3 of 3) |

---

## 🚀 Usage

1. Download `weather.html`
2. Open it in any modern browser (Chrome, Firefox, Safari, Edge)
3. Type a city name in the search bar and press **Enter**
4. Choose your city from the results list
5. Star ⭐ cities you want to save for quick access later

No installation, no build step, no internet-hosted server needed beyond the free API calls.

---

## 🏗️ Tech Stack

- **Pure HTML, CSS, JavaScript** — zero frameworks, zero dependencies
- **Canvas API** — animated weather particle background
- **SVG** — temperature sparkline chart, sun arc, wind compass
- **localStorage** — favorites and search history persistence
- **CSS custom properties** — full design token system for easy theming

---

## 📁 File Structure

```
weather.html   ← entire app, self-contained single file (~700 lines)
README.md      ← this file
```

---

## 📄 License

Open source — free to use, modify, and distribute.
