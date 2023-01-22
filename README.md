# Weather API

This project is a weather API that utilizes data from the OpenWeatherMap API to provide current weather information for a given location.

# Steps
1. Create an account in the OpenWeatherMap website
2. Generate your API key
3. Install the requests library using the command line, pip install requests

## Usage

The API takes two parameters:
- `api_key`: Your OpenWeatherMap API key
- `location`: The location for which you want to retrieve weather information, in the format "city,country code"

Example:
```python
import requests

api_key = "your_api_key"
location = "San Francisco,us"

response = requests.get(f"http://api.openweathermap.org/data/2.5/weather?q={location}&appid={api_key}")

print(response.json())
