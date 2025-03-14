
## Telegram bot: @Mike_WeatherBot
Status of Last Deployment:<br>
<img src="https://github.com/mikerockin/weather_bot/workflows/Deploy to PythonAnywhere/badge.svg? branch=main"><br>
<a href="https://codeclimate.com/github/mikerockin/My_Weather_Bot/maintainability"><img src="https://api.codeclimate.com/v1/badges/400b3120991f564ffe77/maintainability" /></a>

Weather telegram bot, for the entered city can show the weather: for today, tomorrow and three days ahead,
after each forecast returns a voice message with the announced weather forecast (convenient when driving a car),
a request with the name of the city is saved in the database.

1. Returns the following parameters:
2. Weather conditions (snow, rain, cloudy, etc.)
3. Air temperature.
4. Wind speed.
5. Atmospheric pressure.
6. Humidity.
7. Dawn.
8. Sunset.
9. Time zone.

**Features**:
- Written on pure request queries using the weather service "OpenWeathermap";
- Working on www.pythonanywhere.com, restarts via internal tasks pythonanywhere;
- Deployment with Github Actions:
- The application container is available on Docker Hub under the name: mikerockin1988/my-bot

  https://hub.docker.com/r/mikerockin1988/my-bot
  
      $ docker pull mikerockin1988/my-bot:1.0.0
  *After pulling the image, run the container with the command:
  
      $ docker run -d -e TELEGRAM_BOT_TOKEN=YOUR_TOKEN -e OPENWEATHERMAP_API_KEY=YOUR_APID mikerockin1988/my-bot:1.0.0
- The application container is available on Container Registry ( Yandex Cloud ), access to the Docker image for authorized Yandex Cloud users who are members of the organization**

      $ docker pull cr.yandex/crpv85vhagh6a4tpo9mi/my-bot:1.0.0
