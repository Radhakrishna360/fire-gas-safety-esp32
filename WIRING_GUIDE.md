# Wiring Guide – ESP32 Fire & Gas Safety System

## 1. ESP32 DevKit V1

The ESP32 acts as the central processing unit. It reads the sensors, processes the hazard conditions and controls the alarm, LCD, GPS, audio module and monitoring interfaces.

## 2. MQ-2 Gas Sensor

| MQ-2 Pin | ESP32 |
|---|---|
| VCC | 5V |
| GND | GND |
| AO | GPIO34 |

The analog output is monitored by the ESP32 to detect gas/smoke levels against the configured threshold.

**Safety:** Ensure the analog voltage reaching GPIO34 does not exceed 3.3V. Use a voltage divider if required.

## 3. Flame Sensor

| Flame Sensor Pin | ESP32 |
|---|---|
| VCC | Module-rated supply |
| GND | GND |
| DO | GPIO27 |

The digital output is used to identify flame detection according to the sensor's output polarity.

## 4. Buzzer

| Buzzer Connection | ESP32 |
|---|---|
| Signal | GPIO26 |

A transistor driver may be required depending on the buzzer's current requirements.

## 5. LCD 16×2 I2C

| LCD Pin | ESP32 |
|---|---|
| SDA | GPIO21 |
| SCL | GPIO22 |
| VCC | Appropriate supply |
| GND | GND |

The LCD displays the system status and sensor-related information.

I2C address: `0x27`

Check I2C signal voltage compatibility before connecting.

## 6. NEO-6M GPS

| GPS Pin | ESP32 |
|---|---|
| TX | GPIO16 |
| RX | GPIO17 |
| VCC | Module-rated supply |
| GND | GND |

GPS serial configuration: 9600 baud.

The GPS module supplies location information for alert messages.

## 7. DFPlayer Mini

| DFPlayer Pin | ESP32 |
|---|---|
| TX | GPIO25 |
| RX | GPIO33 |
| VCC | 5V |
| GND | GND |
| SPK1 / SPK2 | Speaker |

Serial configuration: 9600 baud.

The DFPlayer Mini plays stored audio alerts corresponding to the hazard conditions.

## 8. Power and Ground

- Use suitable regulated power supplies for the modules.
- Ensure the ESP32 and connected modules share a common ground.
- Protect all ESP32 GPIO signals from voltages above 3.3V.
- Avoid powering high-current modules directly from GPIO pins.
- Verify all connections before powering the system.

## 9. Communication and Monitoring

The ESP32 uses Wi-Fi to communicate with:

- Blynk IoT
- Telegram Bot API
- Local Web Dashboard

The system also provides local alerts and display functions.

## 10. Verification

Check every connection against the pin table and the firmware configuration before powering the circuit.
