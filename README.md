# Weather Dashboard

A Django web app to view current, forecast, and historical weather data using WeatherAPI.com.

## Features

- Search current weather by location
- View 7-day forecast
- View historical weather by date
- Responsive frontend with charts

## Setup

1. **Clone the repository:**
   ```
   git clone repo
   cd weather-dashboard
   ```

2. **Install dependencies:**
   ```
   python -m venv venv
   venv\Scripts\activate   # On Windows
   pip install -r requirements.txt
   ```

3. **Configure environment variables:**
   - Copy `.env.example` to `.env` and add your WeatherAPI key:
     ```
     cp .env.example .env
     ```
     Edit `.env` and set `WEATHER_API_KEY`.

   - **Add your Django secret key to `.env`:**
     ```
     DJANGO_SECRET_KEY=your-secret-key-here
     ```
     Replace `your-secret-key-here` with a secure, random string.

   - **Apply the secret key in your Django settings:**
     In `weather_project/settings.py`, load the secret key from the environment:
     ```python
     import os
     SECRET_KEY = os.getenv('DJANGO_SECRET_KEY')
     ```

4. **Apply migrations:**
   ```
   python manage.py migrate
   ```

5. **Run the development server:**
   ```
   python manage.py runserver
   ```

6. **Access the app:**
   - Open [http://127.0.0.1:8000/](http://127.0.0.1:8000/) in your browser.

## Notes
- You need a free API key from [WeatherAPI.com](https://www.weatherapi.com/).
- Keep your Django secret key private and never commit it to version control.

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