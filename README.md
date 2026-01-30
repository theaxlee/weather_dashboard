# Weather Dashboard

A Django web app to view current, forecast, and historical weather data using WeatherAPI.com.
 
![forecast.png](https://github.com/Madpsych0/weather_dashboard/blob/main/forecast.png)
![forecast.png](https://github.com/Madpsych0/weather_dashboard/blob/main/history.png)
## Features

- Search current weather by location
- View 7-day forecast
- View historical weather by date
- Responsive frontend with charts

## Setup

### 1. Clone the Repository

```bash
git clone https://github.com/Madpsych0/weather_dashboard
cd weather-dashboard
```

### 2. Create & Activate Virtual Environment

#### Windows
```bash
python -m venv venv
venv\Scripts\activate
```
#### macOS / Linux
```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Create `.env` File

Create a `filename.env` in the directory.
Open `.env` in a text editor and set the following values:

```env
WEATHER_API_KEY=your_weather_api_key_here
DJANGO_SECRET_KEY=your_secret_key_here
```

- **WEATHER_API_KEY** → Obtain from your weather API provider.
- **DJANGO_SECRET_KEY** → Generate a long random string (at least 32 characters).

### 5. Apply Database Migrations

```bash
python manage.py migrate
```

### 6. Run the Development Server

```bash
python manage.py runserver
```

## Notes
- You need a free API key from [WeatherAPI.com](https://www.weatherapi.com/).

## Authors

- [@Madpsycho](https://www.github.com/Madpsych0)
- [@theaxlee](https://www.github.com/theaxlee)

## License

MIT License

Copyright (c) 2025 Madpsych0

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
