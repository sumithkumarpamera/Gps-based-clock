# GPS Based Clock System

## Project Title

**GPS CLOCK SYSTEM USING LAUNCHXLTMS320F28379D**

## Project Overview

The **GPS Based Clock System** is an embedded system that receives accurate time information from GPS satellites and displays the synchronized time and date on an OLED display.

The GPS module sends **NMEA sentences** through serial communication. The microcontroller receives and processes the NMEA data, extracts the required time information, converts the UTC time into **Indian Standard Time (IST)**, and displays the result on the OLED.

This system reduces the need for manual time setting and provides accurate, continuously synchronized time.

## Devices / Hardware Used
| **Hardware Device**        | **Purpose in Project**                                         |
| -------------------------- | -------------------------------------------------------------- |
| GPS Module                 | Receives satellite signals and provides accurate time and date |
| TMS320F28379D LaunchPad    | Processes GPS data and controls the OLED                       |
| GPS Antenna                | Receives signals from GPS satellites                           |
| OLED Display               | Displays synchronized time and date                            |
| Power Supply (5V / 3.3V)   | Provides power to system components                            |
| USB Cable / JTAG Interface | Programming and debugging                                      |
| Connecting Wires           | Hardware connections                                           |
| Breadboard / PCB           | Hardware assembly                                              |


## Software / Technologies Used

* Embedded C
* Code Composer Studio (CCS)
* NMEA GPS Protocol
* Serial Communication
* SPI Communication
* GPIO
* OLED Interface

## Working Principle

1. The **GPS module** receives signals from GPS satellites.
2. The GPS module generates **NMEA sentences** containing time, date and location information.
3. The **TMS320F28379D** receives the NMEA data through serial communication.
4. The firmware identifies the required GPS sentence, such as **RMC**, and extracts the UTC time and date.
5. The UTC time is converted to **IST (UTC + 5:30)**.
6. The processed time and date are sent to the **OLED display**.
7. The OLED continuously displays the synchronized time.

## Key Features

* GPS-based automatic time synchronization
* No manual time setting required
* UTC to IST conversion
* Time and date display
* NMEA sentence processing
* Serial communication with GPS module
* OLED-based real-time display
* Embedded C firmware implementation

## My Contribution

* Interfaced the GPS module with the microcontroller.
* Developed Embedded C firmware for receiving and processing NMEA data.
* Implemented GPS time extraction and UTC-to-IST conversion.
* Interfaced the OLED display for showing time and date.
* Worked on serial and SPI communication.
* Performed debugging, testing and system validation.

## Applications

* Railway and transportation systems
* Communication systems
* Navigation systems
* Embedded timing systems
* Industrial systems requiring synchronized time
* GPS-based monitoring systems
