# Spotify Recently Played Tracks ETL

This repository contains a Python script for extracting information about recently played tracks from the Spotify API, transforming the data, and loading it into a SQLite database. This process is often referred to as ETL (Extract, Transform, Load).

## Getting Started

These instructions will help you get a copy of the project up and running on your local machine.

### Prerequisites

Before you begin, make sure you have the following:

- Python 3.x installed on your machine.
- The required Python packages. Install them using the following command:


### Setup

1. Clone the repository to your local machine using Git.

2. Open the `main.py` file and replace the placeholders for `USER_ID` and `TOKEN` with your Spotify username and API token. You can generate your token from the [Spotify Developer Dashboard](https://developer.spotify.com/dashboard/applications).

3. Run the script using the following command:


The script will extract information about your recently played tracks, transform the data, and load it into a SQLite database.

## How It Works

1. The script uses the Spotify API to retrieve information about recently played tracks using the provided API token.
2. The retrieved data is transformed into a pandas DataFrame, and several data quality checks are performed, including checking for empty data, duplicate entries, null values, and timestamp validity.
3. The transformed data is then loaded into a SQLite database. If the data already exists in the database, it will be appended.






