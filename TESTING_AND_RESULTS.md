# Testing and Results

## 1. Testing Objective

The objective of testing is to verify the operation of the ESP32 Fire & Gas Safety System, including sensor detection, local alerts, GPS functionality, communication services, dashboard monitoring and manual override.

## 2. Test Cases and Results

| Test ID | Test Description | Expected Result | Actual Result |
|---|---|---|---|
| T01 | Power-on initialization | ESP32 initializes connected modules | PASS – Verified on hardware |
| T02 | MQ-2 smoke/gas test | Sensor reading increases and hazard status is detected when threshold is crossed | PASS – Verified on hardware |
| T03 | Flame sensor test | Flame condition is detected | PASS – Verified on hardware |
| T04 | Smoke alert | Buzzer and audio warning activate according to programmed logic | PASS – Verified on hardware |
| T05 | Flame alert | Fire alert is triggered | PASS – Verified on hardware |
| T06 | Combined smoke and flame | Combined hazard condition is identified | PASS – Verified on hardware |
| T07 | LCD display | Sensor and system status are displayed | PASS – Verified on hardware |
| T08 | GPS functionality | GPS coordinates are obtained when satellite reception is available | PASS – Verified on hardware |
| T09 | Telegram alert | Alert message is delivered when internet and Telegram connectivity are available | PASS – Verified on hardware |
| T10 | Blynk monitoring | Sensor and status values are updated on the Blynk dashboard | PASS – Verified on hardware |
| T11 | Local web dashboard | Dashboard is accessible over the configured network | PASS – Verified on hardware |
| T12 | Manual override | Buzzer and DFPlayer are silenced according to override logic | PASS – Verified on hardware |
| T13 | Wi-Fi disconnection | Local monitoring and alert functions behave according to firmware logic | PASS – Verified on hardware |
| T14 | Wi-Fi reconnection | Network services reconnect when connectivity returns, as supported by firmware | PASS – Verified on hardware |

## 3. Testing Evidence

The following evidence can be included to demonstrate the prototype's functionality:

- Photographs of MQ-2 sensor testing
- Flame detection demonstration
- LCD status display
- GPS location output
- Telegram alert screenshots
- Blynk dashboard screenshots
- Local web dashboard screenshots
- Manual override demonstration

## 4. Testing Summary

The prototype was tested for sensor detection, alarm response, display operation, GPS functionality, cloud monitoring, Telegram notifications, local web dashboard operation, manual override and network connectivity behavior.

The tested functionalities operated as expected during the hardware demonstration.

## 5. Limitations

- MQ-2 is a general gas sensor and is not a certified fire safety instrument.
- GPS accuracy and availability depend on satellite reception and environmental conditions.
- Telegram, Blynk and remote web services require network connectivity.
- The prototype is intended for educational demonstration and is not a certified life-safety system.
