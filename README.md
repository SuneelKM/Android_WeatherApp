# Project 2 - Weather App

## Project Description
A Android application that allows users to recieve live weather data.

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
* OpenWeather One Call API 3.0 (https://openweathermap.org/api/one-call-3) to get live weather data
* OpenCage Geocoding API (https://opencagedata.com) for reverse geocoding
* Google cloud API key (https://console.cloud.google.com) for Google Place Autocomplete and Google Geocoding
* Google Firebase crahlytics (https://console.firebase.google.com) to monitor and analyze the crashes

## Screenshots

<img src = "https://github.com/SuneelKM/Android_WeatherApp/blob/main/screenshot/WeatherImage.png" width=1200 height=450>

## Features
* Detect your current location based on your IP address
* Has bottom navigation with three pages:
  - Today page: - Contains current weather details for users current location and searched location
  - Weekly page: - Contains weather details for the next 7 days
  - Location page: - Can insert or deleted favourite locations
* Search bar uses Google's Places Autocomplete, so user can start typing a location and autocomplete will provide a list of place predictions
* Can convert the temperature units from Celsius to Fahrenheit
* Dynamic weather icons that correspond to the weather details


## To run the App
* Get the required API keys mentioned above
* Clone the Repo
* When openning the Repo first time in Android Studio, gradle sync will fail. You will need to put the necessary API keys in local.properties file
* In the local.properties file, under sdk.dir line, enter your API keys as show below:
```bash
googleApi = "Your Google Cloud API key"
weatherApiKey = "Your OpenWeather One Call API 3.0 Key"
openCageDataKey = "Your OpenCageDataKey"
```
* Signup for Firebase crahlytics on https://console.firebase.google.com/ and paste your google-services.json file in the "app" folder
* Rebuild your Gradle
* Enjoy!!
