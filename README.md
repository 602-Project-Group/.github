# Aircraft Localization Project

## Team Members
- Taner Bulbul
- Rayyan Waseem
- Dina Hadj-Mabrouk
- Rida Javed Kutty
- Yog Dharaskar

## Project Overview
This project aims to use sensor data and signal strength to locate missing location data of aircraft. We are participating in the CYD Campus Aircraft Localization Competition.

## Repository
Our project code can be found at: [https://github.com/602-Project-Group](https://github.com/602-Project-Group)

## Data Sources
- Competition Dataset: [AIcrowd Challenge Dataset](https://www.aicrowd.com/challenges/cyd-campus-aircraft-localization-competition/dataset_files)
- Documentation:
  - [CYD Campus Aircraft Localization Competition](https://www.aicrowd.com/challenges/cyd-campus-aircraft-localization-competition)
  - [OpenSky Network Competition](https://competition.opensky-network.org/documentation.html)

## Pre-Processing Steps

### Outlier Removal
- Filter outliers in longitude and latitude data
- Apply a filter based on the median value for each aircraft track

### Altitude Data Cleaning
- Create a relationship between Barometric and geometric altitude
- Identify and handle outlier altitude data

### Time Measurement Preprocessing
- Convert raw time measurements (T0) to "true" time measurements (T)
- Use speed of light and 3D distance between aircraft and stations for conversion

### Station Selection
- Select stations providing measurements for the test set
- Create dictionaries to map station numbers and store station locations

### Velocity Calculation
- Predict aircraft velocity using sensor time data and known localization
