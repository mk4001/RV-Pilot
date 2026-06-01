# RV‑Pilot – Aviation Instruments for iOS & CarPlay

[![Swift](https://img.shields.io/badge/Swift-5.9-orange)](https://swift.org)
[![Platform](https://img.shields.io/badge/Platform-iOS%20%7C%20CarPlay-blue)](https://developer.apple.com/carplay/)
[![License](https://img.shields.io/badge/License-MIT-lightgrey)](LICENSE)

**RV‑Pilot** is a professional altimeter and attitude indicator for iPhone, iPad, and CarPlay.  
Perfect for recreational flying, paragliding, hot‑air balloons, hiking – anywhere you need altitude, vertical speed, pressure, and attitude.

## Features

- **GPS Altitude** – absolute MSL altitude with accuracy indication  
- **Barometric Altitude** – derived from atmospheric pressure (ISA formula, QNH 1013.25 hPa)  
- **Pressure** – real‑time barometric reading in hPa or inHg  
- **Magnetic Heading** – same engine as Apple’s Compass app  
- **Pitch & Roll** – device attitude with an interactive bubble level  
- **Ground Speed** – horizontal speed (km/h, mph, kn)  
- **Vertical Speed** – rate of climb/descent (m/s or ft/min)  
- **Voice Alerts** – fully customisable spoken warnings (thresholds & messages) – audio plays through car speakers  
- **CarPlay** – full support:  
  - Main CarPlay scene with three tabs (Navigation, Altitude, Level)  
  - Dashboard scene (instrument cluster) with a compact coloured‑cell layout  
- **Unit Systems** – Metric (m, km/h, hPa), Imperial (ft, mph, inHg), Nautical (ft, kn, hPa)  
- **Privacy First** – no data collection, no tracking, everything runs on‑device

## Requirements

- iOS 14.0 or later (required for CarPlay Dashboard)  
- Xcode 14+ (Swift 5.9)  
- Device with GPS, barometer, and magnetometer (iPhone 6 or newer)  
- For CarPlay: a compatible car and a USB / wireless connection


## Usage on iPhone

Grant Location permission (required for GPS, speed, heading)
The main screen immediately shows altitude, speed, attitude
Tap the ⚙️ gear icon to configure:

Units of measure
Voice selection (language, premium voices, preview)
Alert thresholds and custom messages (use {value} as a placeholder)
Tap the ℹ️ info icon to view app details and privacy statement

## CarPlay

Once your device is connected to the car:

The RV‑Pilot icon appears in the CarPlay launcher
Three tabs are available:

Navigation – speed, vertical speed, heading
Altitude – GPS altitude, barometric altitude, pressure
Level – pitch and roll
The Dashboard (instrument cluster view, if supported by the car) shows a compact grid with essential values
Voice alerts are automatically routed to the car’s audio system

## Architecture

UIKit – iPhone/iPad user interface
CarPlay – both template‑based and dashboard scenes
CoreLocation – GPS, heading, ground speed
CoreMotion – barometric pressure (CMAltimeter) and device attitude (CMMotionManager)
AVFoundation – speech synthesis for voice alerts
Combine – reactive data flow from sensors to UI
UserDefaults – persistent settings

## Contributing

Bug reports and feature requests are welcome via GitHub Issues.
To contribute code:

Fork the repository
Create a feature branch
Submit a pull request
License

This project is released under the MIT License – see the LICENSE file for details.

Contact

For support or questions, please open an issue or use the email provided inside the app’s About screen.
