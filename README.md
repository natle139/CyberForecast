# CyberForecast

CyberForecast is a macOS desktop widget that shows the weather on a green-on-black screen, like an old computer terminal. It shows live data from OpenWeather and updates every 30 minutes.

## What it shows

The widget comes in three sizes, and each larger size adds more information.

- **Small:** the city, the current temperature and conditions, and today's high and low.
- **Medium:** everything in the small size, plus the date, the time, and a forecast for the next four hours.
- **Large:** everything in the medium size, plus the UV index, humidity, sunrise and sunset times, and a forecast for the next two days.

## Good to know

- The location is currently fixed to Sydney.
- OpenWeather's free plan doesn't include the UV index, so the widget estimates it from the time of day and the amount of cloud.
- If the weather can't be loaded, the widget shows sample data until the next update.

## Running it

Open `WeatherWidget.xcodeproj` in Xcode 26 or later on macOS 26.3 or later, add your [OpenWeather API key](https://openweathermap.org/api) in `CyberForecast/WeatherService.swift`, and run the `WeatherWidget` scheme. Then right-click the desktop, choose **Edit Widgets**, and add **CyberForecast**.
