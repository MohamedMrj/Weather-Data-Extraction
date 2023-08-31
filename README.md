
# Weather Data Extraction and Database Management App
![db](https://github.com/MohamedMrj/Weather-Data-Extraction/assets/113178714/5e18886c-c093-4695-bbfe-dca71c89e831)
![qw](https://github.com/MohamedMrj/Weather-Data-Extraction/assets/113178714/d5aecde0-e3a6-41eb-a594-576e325e05ce)

![App Screenshot](screenshot.png) <!-- Replace with an actual screenshot of your app -->

This repository contains a Python application built with Kivy and KivyMD that extracts weather data from websites like "timeanddate.com" and "wunderground.com." The extracted data is then stored in both a Firebase database and an SQLite database. Additionally, there is a second part of the app for general database operations.

## Table of Contents

- [Features](#features)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Application Structure](#application-structure)
- [Database Operations](#database-operations)
- [Contributing](#contributing)
- [License](#license)

## Features

- **Weather Data Extraction**:
  - Extracts weather data such as temperature, humidity, pressure, and visibility from "timeanddate.com" and "wunderground.com."
  - Handles errors and fallbacks to the second website if data is not found on the first.

- **Database Management**:
  - Stores extracted weather data in both a Firebase real-time database and an SQLite database.
  - Supports CRUD (Create, Read, Update, Delete) operations for managing data in the Firebase database.

- **User Interface**:
  - Provides a user-friendly interface built with KivyMD.
  - Allows users to input city and country names to fetch weather data.
  - Displays weather information in a clean and organized manner.

## Prerequisites

Before you begin, ensure you have met the following requirements:

- Python 3.7 or higher installed on your system.
- The following Python packages installed (you can install them using `pip`):
  - `requests`: For making HTTP requests.
  - `beautifulsoup4`: For parsing HTML content.
  - `kivy` and `kivymd`: For the graphical user interface.
  - `sqlite3`: For working with SQLite databases.

## Installation

To install and run this application, follow these steps:

1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/your-username/weather-data-app.git
   cd weather-data-app
   ```

2. Create a virtual environment (recommended but optional):

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install the required Python packages:

   ```bash
   pip install -r requirements.txt
   ```

## Usage

### Weather Data Extraction

1. Run the application:

   ```bash
   python main.py
   ```

2. In the application's interface, enter the **city name** and **country name** for which you want to fetch weather data.

3. Click the **SEARCH** button to extract and display weather information.

### Database Operations (Optional)

This part of the application is for general database operations. It appears to manage a Firebase database. To use this feature:

1. Navigate to the "DB" folder:

   ```bash
   cd DB
   ```

2. Run the database management application:

   ```bash
   python main.py
   ```

3. Use the provided interface to perform GET, POST, PATCH, PUT, and DELETE operations on the Firebase database.

## Application Structure

- `main.py`: Contains the main application logic for weather data extraction and management.
- `main.kv`: Contains the Kivy language markup for the user interface of the weather data extraction part.
- `countries.py`: Contains a dictionary mapping country codes to country names.
- `DB/main.py` and `DB/main.kv`: Contain the application logic and UI for general database operations.
- `requirements.txt`: Lists the required Python packages.

## Contributing

Contributions are welcome! If you'd like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or bug fix: `git checkout -b feature/your-feature-name`
3. Make your changes and commit them: `git commit -m "Add your message here"`
4. Push to your branch: `git push origin feature/your-feature-name`
5. Open a pull request against the `main` branch of this repository.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
