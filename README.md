Leaflet.WeatherIconsLayer
=========================

Current weather icons layer for Leaflet, based on [OpenWeatherMap API](http://openweathermap.org/current).
Partial rework of [outdated sample script](http://openweathermap.org/js/leaflet-layer.js) from OpenWeatherMap site.

As an OpenWeatherMap derivative work, licenced with [Creative Commons BY-SA 2.0](http://creativecommons.org/licenses/by-sa/2.0/). OpenWeatherMap [Terms of service](http://openweathermap.org/terms) apply.

Usage
-----

    map.addLayer(new L.WeatherIconsLayer());

Also, several options available. Here are the defaults shown:

    map.addLayer(new L.WeatherIconsLayer({
        host: 'http://openweathermap.org/',   // API host
        i18n: {...},                          // object with translation strings, see code
        units: 'metric',                      // or 'imperial'; temperature scale
        temperatureDigits: 0,                 // how many decimal digits in temperature
        maxAgeSeconds: 24*60*60,              // 24h; how long the weather data is considered worth showing
    }));
