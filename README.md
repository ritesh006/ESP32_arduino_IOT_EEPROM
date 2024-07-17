# ESP32_arduino_IOT_EEPROM

## Overview

This project demonstrates the use of an ESP32 microcontroller to implement IoT functionalities using Arduino. The project integrates various IoT services, including ESP Rainmaker, Alexa, Google, and IR (Infrared) communication. It also utilizes EEPROM for storing persistent data.

## Features

- **ESP Rainmaker Integration**: Control and monitor your ESP32 device remotely using the ESP Rainmaker cloud service.
- **Alexa Integration**: Use Amazon Alexa to control the ESP32 device with voice commands.
- **Google Integration**: Control the ESP32 device using Google Assistant.
- **IR Communication**: Send and receive infrared signals for remote control applications.
- **EEPROM Usage**: Store and retrieve data in the EEPROM for persistent storage across reboots.

## Hardware Requirements

- ESP32 Development Board
- IR Transmitter and Receiver (optional)
- Micro USB Cable
- Internet Connection

## Software Requirements

- [Arduino IDE](https://www.arduino.cc/en/Main/Software)
- [ESP32 Board Package](https://github.com/espressif/arduino-esp32)
- [ESP Rainmaker Library](https://github.com/espressif/esp-rainmaker)
- [ArduinoJson Library](https://github.com/bblanchon/ArduinoJson)
- [IRremoteESP8266 Library](https://github.com/crankyoldgit/IRremoteESP8266)

## Installation

### Arduino IDE Setup

1. **Install Arduino IDE**:
   - Download and install the latest version of Arduino IDE from [here](https://www.arduino.cc/en/Main/Software).

2. **Install ESP32 Board Package**:
   - Open Arduino IDE.
   - Go to `File` > `Preferences`.
   - In the "Additional Board Manager URLs" field, add the following URL: `https://dl.espressif.com/dl/package_esp32_index.json`.
   - Go to `Tools` > `Board` > `Boards Manager`.
   - Search for "ESP32" and install the package.

3. **Install Required Libraries**:
   - Go to `Sketch` > `Include Library` > `Manage Libraries`.
   - Search for and install the following libraries:
     - ESP Rainmaker
     - ArduinoJson
     - IRremoteESP8266

### Clone the Repository

1. Clone the repository to your local machine:
   ```sh
   git clone https://github.com/yourusername/ESP32_arduino_IOT_EEPROM.git
  ```sh
## Configuration

### ESP Rainmaker

1. Sign up for an account on [ESP Rainmaker](https://rainmaker.espressif.com/).
2. Follow the [ESP Rainmaker setup guide](https://rainmaker.espressif.com/docs/get-started.html) to create a new device and get the necessary credentials.
3. Update the `rainmaker_credentials.h` file in the project with your credentials.

### Alexa and Google Integration

1. Follow the respective guides to set up Alexa and Google Assistant with your ESP32 device.
2. Update the `alexa_google_credentials.h` file with your credentials and settings.

## Usage

### Upload the Code

1. Connect your ESP32 board to your computer using a micro USB cable.
2. Select the correct board and port in Arduino IDE (`Tools` > `Board` > `ESP32 Dev Module` and `Tools` > `Port`).
3. Click the upload button to compile and upload the code to the ESP32.

### Monitor the Serial Output

1. Open the Serial Monitor in Arduino IDE (`Tools` > `Serial Monitor`).
2. Set the baud rate to 115200.
3. Monitor the output for connection status and debug information.

### Control the Device

1. Use the ESP Rainmaker app, Alexa, or Google Assistant to control your device.
2. If using IR, point your IR remote at the ESP32 and press buttons to send commands.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [ESP Rainmaker](https://rainmaker.espressif.com/)
- [ArduinoJson](https://github.com/bblanchon/ArduinoJson)
- [IRremoteESP8266](https://github.com/crankyoldgit/IRremoteESP8266)
