{% raw %} 
---
title: /weatherdata
type: get
description: Get weather forecast by Latitude and Longitude. 
parameters:
  title: Weatherdata parameters
  data:
    - lat:
      - string
      - Required. Latitude.
    - lng:
      - string
      - Required. Longitude.
right_code:
  return: |
  [
  {
  "query": {
    "count": 1,
    "created": "2014-05-03T03:57:53Z",
    "lang": "en-US",
    "results": {
      "channel": {
        "title": "Yahoo! Weather - Tebrau, MY",
        "link": "http://us.rd.yahoo.com/dailynews/rss/weather/Tebrau__MY/*http://weather.yahoo.com/forecast/MYXX0004_c.html",
        "description": "Yahoo! Weather for Tebrau, MY",
        "language": "en-us",
        "lastBuildDate": "Sat, 03 May 2014 11:00 am MYT",
        "ttl": "60",
        "location": {
          "city": "Tebrau",
          "country": "Malaysia",
          "region": ""
        },
        "units": {
          "distance": "km",
          "pressure": "mb",
          "speed": "km/h",
          "temperature": "C"
        },
        "wind": {
          "chill": "32",
          "direction": "170",
          "speed": "4.83"
        },
        "atmosphere": {
          "humidity": "66",
          "pressure": "982.05",
          "rising": "0",
          "visibility": "9.99"
        },
        "astronomy": {
          "sunrise": "6:57 am",
          "sunset": "7:06 pm"
        },
        "image": {
          "title": "Yahoo! Weather",
          "width": "142",
          "height": "18",
          "link": "http://weather.yahoo.com",
          "url": "http://l.yimg.com/a/i/brand/purplelogo//uh/us/news-wea.gif"
        },
        "item": {
          "title": "Conditions for Tebrau, MY at 11:00 am MYT",
          "lat": "1.58",
          "long": "103.74",
          "link": "http://us.rd.yahoo.com/dailynews/rss/weather/Tebrau__MY/*http://weather.yahoo.com/forecast/MYXX0004_c.html",
          "pubDate": "Sat, 03 May 2014 11:00 am MYT",
          "condition": {
            "code": "28",
            "date": "Sat, 03 May 2014 11:00 am MYT",
            "temp": "32",
            "text": "Mostly Cloudy"
          },
          "description": "\n<img src=\"http://l.yimg.com/a/i/us/we/52/28.gif\"/><br />\n<b>Current Conditions:</b><br />\nMostly Cloudy, 32 C<BR />\n<BR /><b>Forecast:</b><BR />\nSat - Scattered Thunderstorms. High: 32 Low: 26<br />\nSun - Thunderstorms. High: 33 Low: 27<br />\nMon - Scattered Thunderstorms. High: 32 Low: 26<br />\nTue - Thunderstorms. High: 32 Low: 26<br />\nWed - Scattered Thunderstorms. High: 32 Low: 27<br />\n<br />\n<a href=\"http://us.rd.yahoo.com/dailynews/rss/weather/Tebrau__MY/*http://weather.yahoo.com/forecast/MYXX0004_c.html\">Full Forecast at Yahoo! Weather</a><BR/><BR/>\n(provided by <a href=\"http://www.weather.com\" >The Weather Channel</a>)<br/>\n",
          "forecast": [
            {
              "code": "38",
              "date": "3 May 2014",
              "day": "Sat",
              "high": "32",
              "low": "26",
              "text": "Scattered Thunderstorms"
            },
            {
              "code": "4",
              "date": "4 May 2014",
              "day": "Sun",
              "high": "33",
              "low": "27",
              "text": "Thunderstorms"
            },
            {
              "code": "38",
              "date": "5 May 2014",
              "day": "Mon",
              "high": "32",
              "low": "26",
              "text": "Scattered Thunderstorms"
            },
            {
              "code": "4",
              "date": "6 May 2014",
              "day": "Tue",
              "high": "32",
              "low": "26",
              "text": "Thunderstorms"
            },
            {
              "code": "38",
              "date": "7 May 2014",
              "day": "Wed",
              "high": "32",
              "low": "27",
              "text": "Scattered Thunderstorms"
            }
          ],
          "guid": {
            "isPermaLink": "false",
            "content": "MYXX0004_2014_05_07_7_00_MYT"
          }
        }
      }
    }
  }
  }
  ]
---

<div class="code-viewer">

<pre data-language="cURL">
curl --get --include 'https://simple-weather.p.mashape.com/weatherdata?lat=1.0&lng=1.0' \
  -H 'X-Mashape-Key: EF3g83pKnzmshgoksF83V6JB6QyTp1cGrrdjsnczTkkYgYrp8p' \
  -H 'Accept: application/json'
  </pre>

</div>
{% endraw %}