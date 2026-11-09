# SDS 510

Project work for SDS 510 at Arizona State University. Command-line work is done using an Ubuntu shell running via WSL (Windows Subsystem for Linux).

**Instructor:** [Alex Halavais](http://alex.halavais.net/bio)

## Module 1: Basic Toolkit

- `bash_session.txt`: bash session recorded with `script`, showing file navigation, `curl`, `tar` and `grep` searches of the data
- `accessed_records.txt`: output of `grep`, which shows the rows whose filename contains "education" and end in ".txt"

The source data (`log.csv`, from `log.tar.gz`) is not included because of its size. To recreate it:

    curl -s -L https://www.dropbox.com/s/14jagxjbzhyxg8g/log.tar.gz -o log.tar.gz
    tar -xzvf log.tar.gz

## Module 2: Python

- `mastodon_basics.ipynb`: searches Mastodon post contents for five keywords (cheese, pickles, buns, meat, sesame) over the past six weeks, using `Mastodon.py`. The API access token is entered with `getpass()`, so it never appears in the notebook.
- `mastodon-hits.csv`: posts collected by the Mastodon notebook
- `python_essentials_open_meteo.ipynb`: pulls historical weather data from the Open-Meteo API for three New Mexico coal-fired generating stations: San Juan, Four Corners, and Escalante. Variables cover precipitation, evapotranspiration, soil moisture, relative humidity, and maximum temperature.
- `nm_coal_weather_daily_2006_2025.csv`: daily weather records for each station, 2006 to 2025
- `nm_coal_weather_annual_2006_2025.csv`: annual totals and averages for each station

## Module 3: Dealing with Data

- `phoenix_crime_basics.ipynb`: groups Phoenix crime records as violent or non-violent using the FBI Uniform Crime Reporting definition, then finds the fastest growing and shrinking zip codes for each group from 2016 to 2024. Each trend runs twice: once with every zip code, and once without zip codes whose small counts skew the percent change.

The source data (`crime-data_crime-data_crimestat.csv`, 71 MB) is not included because of its size. The notebook loads it from Google Drive:
https://drive.google.com/file/d/1sYJDsWaWNumuSCpYrvxBBOFG6yYKLIlL/view?usp=sharing

Original source: [Phoenix Open Data, Crime Data](https://www.phoenixopendata.com/dataset/crime-data)
