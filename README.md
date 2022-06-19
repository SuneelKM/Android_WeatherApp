# Project 2 - Weather App

## Project Description
A simple Android application that allows users to recieve live weather data.

## Technologies Used
* Kotlin
* Android Studio - Chipmunk
* MVVM Design
* RxKotlin
* Room DB 
* Retrofit2 
* Mockito
* JUnit 
* Google Places SDK 
* Firebase Crashlytics
* Timber Tree logger

## APIs Used
* OpenWeather One Call API 3.0 to get live weather data
* OpenCage Geocoding API for reverse geocoding
* Google cloud API key for Google Place Autocomplete and Google Geocoding
* Google Firebase crahlytics to monitor and analyze the crashes

## Screenshots

<img src = "https://github.com/SuneelKM/AndroidWeatherApp/blob/master/Screenshot/image.png" width=1200 height=450>

## Features
* Detect your current location based on your IP address
* Has bottom navigation with three pages:
  - Today page: - Contains current weather details for users current location and searched location
  - Weekly page: - Contains weather details for the next 8 days
  - Location page: - Can insert or deleted favourite locations
* Search bar uses Google's Places Autocomplete, so user can start typing a location and autocomplete will provide a list of place predictions
* Can convert the temperature units from Celsius to Fahrenheit
* Dynamic weather icons that correspond to the weather details


## To run the App
* Get the required API keys mentioned aboved.
* Clone the Repo.
* When openning the Repo first time in Android Studio, gradle sync will fail. You will need to put the necessary API keys in local.properties file.
* In the local.properties file, under sdk.dir line, enter your API keys as show below:
```bash
googleApi = "Your Google Cloud API key"
weatherApiKey = "Your OpenWeather One Call API 3.0 Key"
openCageDataKey = "Your OpenCageDataKey"
```
* Signup for Google firebase crahlytics and paste your google-services.json file in the "app" folder.
* Rebuild your Gradle.
* Enjoy!!
