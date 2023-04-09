# Clima-App
Weather app that is able to check the weather for the current location based on the GPS data from the iPhone as well as by searching for a city manually.

## Table of contents
* [Features](#features)
* [Technologies](#technologies)
* [Condition Codes](#conditioncodes)

## Features 
* Viewing the weather of the location based on the GPS data pulled from API service 
* Searching any city manually for weahter information.

## Technologies
Project is created with:
* Xcode 14.2
* UIKit
* Extension
* Delegate Pattern 
* Protocol
* Core Location
* URL Session

## Condition Codes

```swift

switch conditionID {
        case 200...232:
            return "cloud.bolt"
        case 300...321:
            return "cloud.drizzle"
        case 500...531:
            return "cloud.rain"
        case 600...622:
            return "cloud.snow"
        case 701...781:
            return "cloud.fog"
        case 800:
            return "sun.max"
        case 801...804:
            return "cloud.bolt"
        default:
            return "cloud"
        }
