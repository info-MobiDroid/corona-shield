# Corona-Shield <a href="https://twitter.com/intent/tweet?url=https://github.com/aminejafur/corona-shield" target="_blank">![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social&logo=twitter)</a>

### A Corona Tracking Mobile Application.

Corona Shield is an open sourced Corona Tracking Mobile Application with Back-end made by <a href="https://github.com/aminejafur" target="_blank">Amine Jafur</a> using <a href="https://flutter.dev" target="_blank">Flutter</a>, <a href="https://www.php.net" target="_blank">PHP</a>, <a href="https://developer.mozilla.org/fr/docs/Web/JavaScript" target="_blank">JS</a>.


After watching <a href="https://www.youtube.com/watch?v=xTQoi30OiIc" target="_blank">Najib El Mokhtari's video</a> about the government application project for COVID-19 tracking. And, since I had built a similar bluetooth tracking application for the open-ended Hackathon 2015 by Screendy hosted in Casablanca, I decided to rebuilt the Application by my own from scratch and this is what I came up with.

![Corona Shield Application](https://raw.githubusercontent.com/aminejafur/corona-shield/master/images/mockup2.png)

## Table of Contents

* [Versions](#versions)
* [How It Works](#how-it-works)
* [Video](#video)
* [Screenshots](#screenshots)
* [Quick Start](#quick-start)
* [Licensing](#licensing)
* [Useful Links](#useful-links)

## Versions

First Verison of the APP : 1.0

## How It Works
1. First of all, download the App.
2. Open the app and follow the steps.
3. Signup using your CIN + Phone ( Make sure to have internet ).
4. Activate the bluetooth so the application can get your mac Adresse else you can enter it by your own. 
5. After the signing, you will be redirected to the main page of the application, where you will get the Statistics and your profile details as a card.
6. If you are deciding to go out, Click on the tracking button in the right bottom corner and start tracking any collisions arround you.
7. The app will keep tracking for any persones you meet out there and it will save them in your phone using a spesific encryption.
8. Let's say as example that you got the covid-19 ( EXAMPLE xD ), the gouvernement will take your phone and it will be able to access the encrypted data from your phone using the List icon in the navigation Bar, they can also upload the decrypted data to ther servers to get stastics and find the persones you collided with in a very safe way.

That's All, Stay safe nd Stay #home

## Video

## Screenshots

| Onboarding | Login | Mac Adresse | Main Screen | Radar |
|:---:|:---:|:---:|:---:|:---:|
| <img src="https://raw.githubusercontent.com/aminejafur/corona-shield/master/images/Oboarding.jpg" width="200" height="400"> | <img src="https://raw.githubusercontent.com/aminejafur/corona-shield/master/images/Login.jpg" width="200" height="400"> | <img src="https://raw.githubusercontent.com/aminejafur/corona-shield/master/images/Mac_adresse.jpg" width="200" height="400"> | <img src="https://raw.githubusercontent.com/aminejafur/corona-shield/master/images/Main.jpg" width="200" height="400"> | <img src="https://raw.githubusercontent.com/aminejafur/corona-shield/master/images/Radar.jpg" width="200" height="400"> |

## Quick start

## API 

1 - Create a database.

2 - Go to the /api folder and rename the .env.example file to .env and fill it with the database info.

3 - Open CMD, type : php dbseed.php ( you should get 2 messages, Starting Seed + seeded).

4 - In the same CMD type : php -S YOUR-IP:portShoosedForAPI -t public.

5 - Make sure the API is working fine, visit : YOUR-IP:portShoosedForAPI/users OR YOUR-IP:portShoosedForAPI/collisions.

## STATISTICS

Go to Server file or wherever you moved the "Server/statistics.php" File and open CMD, type php  -S your-IP:portShoosedForStatistics.

## DASHBOARD

<img src="https://raw.githubusercontent.com/aminejafur/corona-shield/master/images/Dashboard.png" width="900" height="500">

1 - Edit the "dashboard\assets\js\config.js" file ( export const apiUrl = 'http://your-IP:portShoosedForDashboard'; ).

2 - Go to dashboard folder and open CMD, type : php -S your-IP:portShoosedForDashboard.

3 - Now your dashboard can be accessed from your-IP:portShoosedForDashboard in your browser.


## Mobile APP

1 - Edit the "mcovid_shield\lib\ui\globalVars.dart" file with :

	- govPassword = the password that will be used to access the collected data, normal user should not access it!.

	- statisticsUrl = your-IP:portShoosedForStatistics/statistics.php.

	- apiUrl = your-IP:portShoosedForAPI.

	- encKey = encryption Key Used for two ways encryption while showing/storing Data.


2 - Build the APK depending on your IDE.

HAPPY HACKING!

## Licensing

- Copyright 2020 <a href="https://github.com/aminejafur" target="_blank">Amine Jafur</a>

## Useful Links

- <a href="https://flutter.dev" target="_blank">Flutter</a>