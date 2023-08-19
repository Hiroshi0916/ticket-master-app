# My Event Application

## Overview

This application is a browser-based system built to search and display event details leveraging the Ticketmaster API. It's structured into three core components: a browser frontend, a Node.js backend, and the Ticketmaster server.
# This is an academic project, so the code is not publicly available. If requested during the hiring process, I will grant access permissions

<img width="1452" alt="スクリーンショット 2023-08-19 午前2 18 49" src="https://github.com/Hiroshi0916/ticket-master-app/assets/25889574/1a5675be-e1dd-4a02-bfd6-b6a3116ee13c">
[See the live application here](https://csci571-hw8-379104.wl.r.appspot.com/search)

## Features & Functionality

### General

- **Backend Implementation**: Built using JavaScript and the Node.js Express framework. Implementations outside of Node.js will result in significant deductions.
- **Frontend Implementation**: Developed with the Angular framework. It is essential to use Angular version 8 or above. React-based implementations are not supported.
- **Responsive Design**: Designed mobile-first using Bootstrap.
- **Cloud Deployment**: Both frontend and backend are deployed in the cloud. The backend serves both the frontend and other endpoints.
- **API Calls**: Calls from the Node.js backend to the Ticketmaster API and others are executed through libraries like `axios()` and `node-fetch()`.
- **Browser Compatibility**: The application will be evaluated on the latest version of the Google Chrome browser.

### Frontend Features

- **Navigation Bar**: Displayed on top across all routes, containing two menu options: `Search` and `Favorites`.
- **Search Route**: Enables searching for event information and displaying details. Consists of components such as the search form, results table, event detail card, and marking an event as a favorite.
- **Favorites Route**: Displays a list of events marked as favorites.
- **Search Form**: Contains five components – Keyword, Distance, Category, Location, and a checkbox for automatic location detection.
    - **Geolocation**: Uses `ipinfo.io` API to obtain user's geolocation.
    - **Autocomplete**: Keyword-based autocomplete feature leveraging the Ticketmaster Suggest API.
- **Location Field**: 
    - Automatically detects user location if the checkbox is checked, disabling the Location textbox.
    - Uses the Google Maps Geocoding API to obtain latitude and longitude for user-inputted locations.
- **Event Search & Display**: 
    - **Geocoding**: Converts user-inputted address to latitude and longitude using the Google Maps Geocoding API.
    - **Event Searching**: Leverages the Ticketmaster API to search for event information.
    - **Error Display**: Shows error tooltips for incomplete input.
    - **Results Display**: Shows up to 20 search results in a tabular format.
    - **Details Card**: Displays event details, artist/team info, venue details, etc., in card format.
    - **Favorites**: Allows saving and deleting favorite events in local storage.
    - **Spotify Integration**: Fetches artist information like popularity, follower count, and album images using the Spotify API.
    - **Venue Information**: Retrieves detailed venue information using the Ticketmaster API.
    - **Google Maps Display**: Displays the venue location on a Google Maps modal.
    - **Responsive**: Ensures the application functions and looks appropriate across mobile devices and various screen sizes.


# Technologies Used

## Frontend

### Angular
- **Version**: 15.0.0
- **Modules Used**: 
  - animations
  - cdk
  - common
  - compiler
  - core
  - forms
  - google-maps
  - material
  - platform-browser
  - platform-browser-dynamic
  - router

### Bootstrap
- **Version**: 5.2.3
- **Extensions**:
  - **bootstrap-icons**: 1.10.3
  - **ngx-bootstrap**: 6.2.0

## Backend

### Node.js
- Utilized for server-side implementation.

### spotify-web-api-node
- **Version**: 5.0.2
- A wrapper for using Spotify's Web API from Node.js.

## Utilities

### rxjs
- **Version**: 7.5.0
- Reactive extensions library for JavaScript.

### tslib
- **Version**: 2.3.0
- Helper library for TypeScript.

### zone.js
- **Version**: 0.12.0
- Library for Angular's automatic change detection.

## Development Tools

### @angular-devkit/build-angular
- CLI tools and devkit for building Angular applications.

### @angular/cli
- Command-line interface for Angular.

### TypeScript
- **Version**: 4.8.2

